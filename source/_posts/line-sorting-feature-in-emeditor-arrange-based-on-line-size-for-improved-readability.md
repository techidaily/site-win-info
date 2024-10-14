---
title: "Line Sorting Feature in EmEditor: Arrange Based on Line Size for Improved Readability"
date: 2024-10-06T18:10:04.317Z
updated: 2024-10-14T09:05:44.182Z
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
<li><a href="https://extra-hints.techidaily.com/new-capture-and-amplify-no-cost-digital-picture-upgrades/"><u>[New] Capture & Amplify - No Cost Digital Picture Upgrades</u></a></li>
<li><a href="https://remote-screen-capture.techidaily.com/new-in-2024-step-by-step-guide-to-iphone-screen-capturing/"><u>[New] In 2024, Step-by-Step Guide to Iphone Screen Capturing</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/updated-3-tactics-to-grab-twitter-gifs-on-pc-for-2024/"><u>[Updated] 3 Tactics to Grab Twitter GIFs on PC for 2024</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/updated-8-free-instagram-to-mp4-converters-you-can-try-onlinewindowsmac/"><u>[Updated] 8 Free Instagram to MP4 Converters You Can Try [Online/Windows/Mac]</u></a></li>
<li><a href="https://howto.techidaily.com/cellular-network-not-available-for-voice-calls-on-samsung-galaxy-m14-4g-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Cellular Network Not Available for Voice Calls On Samsung Galaxy M14 4G | Dr.fone</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/expert-tips-on-utilizing-the-teleport-feature-in-minecraft-gaming/"><u>Expert Tips on Utilizing the Teleport Feature in Minecraft Gaming</u></a></li>
<li><a href="https://review-topics.techidaily.com/how-to-changefake-your-xiaomi-redmi-note-13-5g-location-on-viber-drfone-by-drfone-virtual-android/"><u>How to Change/Fake Your Xiaomi Redmi Note 13 5G Location on Viber | Dr.fone</u></a></li>
<li><a href="https://iphone-transfer.techidaily.com/how-to-copy-contacts-from-apple-iphone-15-pro-max-to-sim-drfone-by-drfone-transfer-from-ios/"><u>How to Copy Contacts from Apple iPhone 15 Pro Max to SIM? | Dr.fone</u></a></li>
<li><a href="https://win-info.techidaily.com/how-to-fix-outline-text-issues-in-emeditor-a-comprehensive-guide/"><u>How to Fix 'Outline Text' Issues in EmEditor: A Comprehensive Guide</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/in-2024-top-tech-reviews-with-a-focus-on-alternatives/"><u>In 2024, Top Tech Reviews with a Focus on Alternatives</u></a></li>
<li><a href="https://win-info.techidaily.com/introducing-emeditor-professional-v13-beta-6-enhanced-text-editing-experience/"><u>Introducing EmEditor Professional v13 Beta 6 - Enhanced Text Editing Experience.</u></a></li>
<li><a href="https://win-info.techidaily.com/overcoming-rendering-challenges-for-ltr-and-rtl-text-during-horizontal-scrolling-in-emeditor/"><u>Overcoming Rendering Challenges for LTR and RTL Text During Horizontal Scrolling in EmEditor</u></a></li>
<li><a href="https://win-info.techidaily.com/potential-syntax-errors-no-worries-with-emeditor-your-reliable-text-editing-companion/"><u>Potential Syntax Errors? No Worries with EmEditor - Your Reliable Text Editing Companion!</u></a></li>
<li><a href="https://win-info.techidaily.com/professional-text-editing-software-emeditor-pro-version-900-beta-update/"><u>Professional Text Editing Software - EmEditor Pro Version 9.00 Beta Update</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2087485/7443" target="_top" id="2087485">
  <img src="//a.impactradius-go.com/display-ad/7443-2087485" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2087485/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

