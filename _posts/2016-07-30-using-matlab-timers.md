---
layout: post
title: <code>Wait()</code> on MATLAB Timer Objects
---

Unsurprisingly, MATLAB's [timer object][timer object] is great for scheduling code to run at specified time intervals.

However, consider the following test case:

```
function [] = timerTest

% initialize a timer
t = timer('TimerFcn',@counter,'Period',1,'TasksToExecute',5,'ExecutionMode','fixedRate');

% keep track of how many times the timer has run
count = 0;

% start timer
start(t);

    % code that is executed on every timer cycle
    function counter(~,~)
        count = count + 1;
    end

% display how many times the timer has run
disp(count);
end
```

I expected that the Command Window would display 5. But it actually displays 1.

Why? It turns out that timers don't automatically block the main thread. After the timer is started, MATLAB continues to execute more code, while keeping track of the timer on the side. When the timer needs execute again, MATLAB stops, executes the timer callback function, and then continues on its way.

But I wanted to process a matrix that the timer first had to populate, meaning that I needed the program to wait until the timer finished until continuing executing more code.[^1]

Turn out, it's just this simple:

```
start(t)
wait(t)
```

Add [`wait()`][wait], and MATLAB will not continue executing code until the timer has finished.

[timer object]: http://www.mathworks.com/help/matlab/ref/timer-class.html
[wait]: http://www.mathworks.com/help/matlab/ref/timer.wait.html?searchHighlight=wait

[^1]: My temporary hack (and I suspect for many others as well) was to add a `pause()` that was as just longer than the expected timer duration.
