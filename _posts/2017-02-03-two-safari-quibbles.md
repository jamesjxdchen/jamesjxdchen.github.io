---
layout: post
title: Two Safari Quibbles
---

As a student, the flexibility of a PC is indispensable. And judging by the technology used by my peers, this is true of near *every* student. However, it is still true that the majority of my computing (maybe ~60%) happens in the web browser.

On macOS, Safari and Google Chrome are the two powerhouse web browsers. Both have support for modern web standards, and both are very extensible. But Safari has two clear advantages: two-finger scrolling responsiveness and power efficiency. The best comparison I can make between two-finger scrolling in the two web browsers is scrolling in Android and iOS. Chrome feels like scrolling in Android: not bad, but not good. Safari feels like scrolling in iOS: fantastic. Once you tinker around in iOS, you realize how janky Android scrolling is (I use a Moto X Android phone). And there might not be a more important feature than power efficiency. Because of how heavily I use the web browser it is often the largest consumer of battery life.

Having listed Safari's advantages over Chrome, there are still two quibbles I have with Safari that keep me using Chrome. And both have to do with the way tabs are displayed in Safari. Note that I have Increase Contrast selected in Accessibility.

![safari-tabs.png](/assets/2017/02/safari-tabs.png)*Safari tabs.*

![chrome-tabs.png](/assets/2017/02/chrome-tabs.png)*Chrome tabs.*

## 1. Lower Contrast Text

First, the text contrast of website titles in Safari is lower than in Chrome, which makes them harder to read. This quibble might be a function of using a non-retina MacBook Air, as I could see a sharper, more color accurate screen alleviating these issues. Even though Safari has lower contrast than Chrome, its text contrast is still above the 7:1 contrast ratio [recommended by Apple][apple contrast ratio].

<div class="table-wrapper">
<table>
  <tr>
    <th>Web Browser</th>
    <th>Contrast Ratio</th>
    <th>Text Color</th>
		<th>Background Color</th>
  </tr>
  <tr>
    <td>Chrome (foreground tab)</td>
    <td>19.1:1</td>
    <td>rgb(0, 0, 0)</td>
		<td>rgb(243, 243, 243)</td>
  </tr>
	<tr>
		<td>Safari (foreground tab)</td>
		<td>14.4:1</td>
		<td>rgb(0, 0, 0)</td>
		<td>rgb(214, 214, 214)</td>
	</tr>
	<tr>
		<td>Chrome (background tab)</td>
		<td>14.3:1</td>
		<td>rgb(0, 0, 0)</td>
		<td>rgb(213, 213, 213)</td>
	</tr>
	<tr>
		<td>Safari (background tab)</td>
		<td>10.7:1</td>
		<td>rgb(0, 0, 0)</td>
		<td>rgb(185, 185, 185)</td>
	</tr>
</table>
</div>

## 2. No Favicons

The decreased legibility of Safari tab labels wouldn't be such a large issue if not exacerbated by my second quibble: no favicons next to website titles.

Here's my reasoning for why Safari does not show favicons. Safari tabs are implemented using native macOS tabs that can be found in TextEdit, Finder, etc. And in every other application, tabs are labeled only with text.

Even so, for me, favicons are the single most important identifier for different tabs. With favicons, I can glance at an icon instead of reading text to figure out which tab is which. Even better, as you navigate to different pages of a website, often the title will change, but the favicon does not. So the favicon offers a certain degree of reliability that text labels do not.

To my point, where appropriate, Apple features icons on many other labels around macOS.

![mac-icons.png](/assets/2017/02/mac-icons.png)*Icons used in System Preferences, Finder, and the "Command-Tab" Application Switcher.*

Even Safari uses the Touch Bar to display favicons, not text labels.

![macbookpro-touch-bar-safari-favorites.png](/assets/2017/02/macbookpro-touch-bar-safari-favorites.png)*Image from [Apple](https://support.apple.com/en-us/HT207055).*

Fingers crossed—🤞🤞—here's to favicons and increased text contrast in Safari tabs.

[apple contrast ratio]: https://developer.apple.com/ios/human-interface-guidelines/visual-design/color/
