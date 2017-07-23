---
layout: post
title: Email as a Bulletin Board
---

Here is how to subscribe to a bulletin board type mailing list, high-volume and low importance, while maintaining your email sanity.

## 1. Bundle It Away

On a high-volume email list like this, most of the emails are totally irrelevant to me. While I want to be able to scan through and catch any interesting upcoming events, I don't want them cluttering up my inbox. So I hide them away.

![inbox-rockywire-example.png](/assets/2015/01/inbox-rockywire-example.png)*This is a typical email.*

For this, I use Google Inbox's [bundling feature][bundling]. I filter out all emails from this email list and show the bundle once per day. Every morning, this bundle will show up in my inbox, and I can quickly scan the subjects and see if anything is of interest. It's a nice daily briefing of interesting events happening around campus.

It's important to make sure that these emails don't reach my viewable inbox as they arrive. It's too easy to check for new emails every 15 minutes, even though they are of minimal importance.

![inbox-bundle.png](/assets/2015/01/inbox-bundle.png)*Here are my bundle settings.*

[bundling]: https://support.google.com/inbox/answer/6050237?hl=en

## 2. Automatically Delete It

This is the critical step. After a month on a real bulletin board, flyers are torn-off, covered up, or rained away. And because people treat these mailing lists like bulletin boards, it makes sense to treat these emails the same. I don't want all of this cruft sitting around in my email. It makes searching more cumbersome and takes up storage space in my inbox.

If Google stores your email, then you can do this by running a script on Google App Engine. I'm using a [script from John Day][script], and I've set the automatic delete time to be 5 days.

[script]: http://www.johneday.com/422/time-based-gmail-filters-with-google-apps-script

## Why Bother

Public bulletin boards are a staple on college campuses.

But more and more, information about campus happenings are advertised online through a combination of mostly Facebook and Email.

Hearing about events through Facebook is great. Things come and go on the timeline. I can scroll through events, keeping note of the interesting ones. There is a very low mental burden of having all these events on my timeline. They just come and go without any hassle.

But using email as a bulletin board is a little more problematic. Fundamentally, email is more like a physical mailbox than a public bulletin board. Ideally, I would like to keep the ratio of information-to-junk as high as possible, which is why I don't subscribe to many promotional mailing lists. I have a higher standard of quality for emails than I do something on Facebook. Keeping the information density as high as possible means that the important emails aren't loss through the fluff.

Plus, coming through a high-volume email list can start to feel like work. Once every two weeks there is an interesting email, but every other email puts an administrative and mental burden on you—forcing me to read, skim, and delete it.

This solution takes that burden away. It coalesces what could be 10s of [context switches][cs] during the day into one nice morning roundup. And you never have to worry about managing any of it.

![inbox-zero.png](/assets/2015/01/inbox-zero.png)*Inbox zero. 😊*

[cs]: http://blog.codinghorror.com/the-multi-tasking-myth/
