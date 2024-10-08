---
title: "Line Sorting Feature in EmEditor: Arrange Based on Line Size for Improved Readability"
date: 2024-10-06T17:10:09.419Z
updated: 2024-10-08T16:41:30.796Z
tags:
  - product
categories:
  - emeditor
thumbnail: https://thmb.techidaily.com/775033cec734e193d493811f769dcaa65d428fba2286e40a488d59f8b08228ae.png
---

## Line Sorting Feature in EmEditor: Arrange Based on Line Size for Improved Readability

Viewing 2 posts - 1 through 2 (of 2 total)

* Author  
Posts
* February 26, 2012 at 4:44 pm [#10085](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/1900479d3983c44c0bc5f8d9d32d55c2?s=80&d=identicon&r=g)user](https://www.emeditor.com/forums/users/user/ "View user's profile")  
Participant  
hello  
 in Emeditor, there is a feature to sort lines alphabetically or arithmetically, but how can I sort lines according to their length?  
 thanks!  
February 27, 2012 at 4:25 am [#10087](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/7b5f4b0747b67d5f8b87e5b7dd57367b?s=80&d=identicon&r=g)zhouzh2](https://www.emeditor.com/forums/users/zhouzh2/ "View zhouzh2's profile")  
Participant  
Hi user,  
 I wrote this macro for you:  
document.selection.EndOfDocument(false);  
	endOfDocu = document.selection.GetActivePointY(eePosView);  
	document.selection.StartOfDocument(false);  
	document.selection.EndOfLine(false,eeLineView);  
	currentCursor = document.selection.GetActivePointY(eePosView);  
	while (endOfDocu != currentCursor) {  
		currentCursor = document.selection.GetActivePointY(eePosView);  
		numberOfChar = document.selection.GetActivePointX(eePosLogical) - 1;  
		document.selection.StartOfLine(false,eeLineView | eeLineHomeText);  
		document.selection.Text=numberOfChar + ": ";  
		document.selection.LineDown(false,1);  
		document.selection.EndOfLine(false,eeLineView);  

	 This macro will add numbers which indicate the number of characters of the line to the start of lines.  
 After that,you can use the “sort” of emeditor.  
 Than replace “^d+?:s” with NULL to restore orginial line.  
 Hope it helps. :-)  
 Cheers,  
 angus.
* Author  
Posts

Viewing 2 posts - 1 through 2 (of 2 total)

* You must be logged in to reply to this topic.

<ins class="adsbygoogle"
     style="display:block"
     data-ad-format="autorelaxed"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="1223367746"></ins>

<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="8358498916"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>

<span class="atpl-alsoreadstyle">Also read:</span>
<div><ul>
<li><a href="https://fox-links.techidaily.com/new-2024-approved-logic-pros-way-to-softly-diminish-loud-passages/"><u>[New] 2024 Approved Logic Pro's Way to Softly Diminish Loud Passages</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/new-top-tips-for-masterful-looped-videos-on-instagram-for-2024/"><u>[New] Top Tips for Masterful Looped Videos on Instagram for 2024</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/updated-sonic-layers-in-reels-weaving-audio-into-visuals/"><u>[Updated] Sonic Layers in Reels Weaving Audio Into Visuals</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/2024-approved-exploring-top-iphone-video-editors-cameo-and-filmorago-face-off/"><u>2024 Approved Exploring Top iPhone Video Editors Cameo & FilmoraGo Face-Off</u></a></li>
<li><a href="https://some-skills.techidaily.com/2024-approved-the-creative-vanguard-top-6-redefining-digital-arts/"><u>2024 Approved The Creative Vanguard Top 6 Redefining Digital Arts</u></a></li>
<li><a href="https://hardware-updates.techidaily.com/get-the-ultimate-deal-on-the-corsair-scimitar-rgb-elite-a-top-tier-mmo-gaming-mouse-at-just-49/"><u>Get the Ultimate Deal on the Corsair Scimitar RGB Elite - A Top-Tier MMO Gaming Mouse at Just $49</u></a></li>
<li><a href="https://unlock-android.techidaily.com/in-2024-downloading-samfw-frp-tool-30-for-itel-by-drfone-android/"><u>In 2024, Downloading SamFw FRP Tool 3.0 for Itel</u></a></li>
<li><a href="https://win-info.techidaily.com/mastering-windows-quick-assist-a-superior-alternative-to-remote-desktop-for-effective-tech-support/"><u>Mastering Windows Quick Assist: A Superior Alternative to Remote Desktop for Effective Tech Support</u></a></li>
<li><a href="https://win-info.techidaily.com/resurrecting-memories-expert-tips-for-accessing-forgotten-passwords-on-old-computers-digital-recovery-with-zdnet/"><u>Resurrecting Memories: Expert Tips for Accessing Forgotten Passwords on Old Computers | Digital Recovery with ZDNet</u></a></li>
<li><a href="https://buynow-tips.techidaily.com/1723026158322-revolutionizing-home-internet-with-amplifi-hd-no-wi-fi-zone-left-behind/"><u>Revolutionizing Home Internet with Amplifi HD - No Wi-Fi Zone Left Behind!</u></a></li>
<li><a href="https://win-info.techidaily.com/secure-your-system-with-these-simple-steps-building-a-winning-windows-recovery-drive/"><u>Secure Your System with These Simple Steps: Building a Winning Windows Recovery Drive</u></a></li>
<li><a href="https://win-info.techidaily.com/the-game-changing-arrival-of-new-apps-for-windows-on-arm-systems/"><u>The Game-Changing Arrival of New Apps for Windows on Arm Systems</u></a></li>
<li><a href="https://buynow-reviews.techidaily.com/the-ultimate-guide-to-choosing-a-great-deal-hisense-50-hdr-tv-review/"><u>The Ultimate Guide to Choosing a Great Deal: Hisense 50 HDR TV Review</u></a></li>
<li><a href="https://win-info.techidaily.com/to-embrace-or-not-to-embrace-android-on-windows-11-a-comprehensive-guide-by-zdnet/"><u>To Embrace or Not to Embrace Android on Windows 11 - A Comprehensive Guide by ZDNet</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2144279/7443" target="_top" id="2144279">
  <img src="//a.impactradius-go.com/display-ad/7443-2144279" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2144279/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

