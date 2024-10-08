---
title: "Creating Your First Macro with EmEditor: Tips and Tricks for Text Editing Automation"
date: 2024-10-01T17:22:44.626Z
updated: 2024-10-08T17:19:06.504Z
tags:
  - product
categories:
  - emeditor
thumbnail: https://thmb.techidaily.com/85be9153d8c81024583588a94ed9e00fc880777ac2a8c7cff5efd5d21044d91c.jpg
---

## Creating Your First Macro with EmEditor: Tips and Tricks for Text Editing Automation

May 13, 2008 at 9:00 pm [#5775](https://tools.techidaily.com/emeditor/products/) 

[![](https://secure.gravatar.com/avatar/967439df4a399c227144f5d67a4a17d2?s=80&d=identicon&r=g)prashob12](https://www.emeditor.com/forums/users/prashob12/ "View prashob12's profile")

Member

Thanks a lot for replying

 I tried what u told, but the number of Empty elements present in the is many, so if i use the replacment option it deletes one instance at a time, and the number of files with such instances are also many, so it will be time consuming.

 I created a macro to replace all empty elements in at one go:

 document.selection.Find(“”,eeFindNext | eeFindReplaceRegExp);  
 document.selection.CharLeft(false,1);  
 editor.ExecuteCommandByID(4153);  
 document.selection.Find(“”,eeFindNext | eeFindReplaceRegExp);  
 document.selection.Replace(“(\]+>){1,20}”,””,eeFindNext | eeReplaceSelOnly | eeReplaceAll | eeFindReplaceRegExp);  
 document.selection.Replace(“”,””,eeFindNext | eeReplaceSelOnly | eeReplaceAll | eeFindReplaceRegExp);  
 document.selection.CharRight(false,1);

 But i dont know how to make it run on all the files.  
 There are 1000’s of such files.

 Thanks in Advance!!

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
<li><a href="https://video-capture.techidaily.com/new-voice-recording-access-review-and-evaluate/"><u>[New] Voice Recording Access, Review & Evaluate</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-explore-the-best-smartphone-compatible-vr/"><u>[Updated] Explore the Best Smartphone-Compatible VR</u></a></li>
<li><a href="https://win-info.techidaily.com/ai-personal-computers-unveiled-making-an-informed-decision-on-purchasing/"><u>AI Personal Computers Unveiled - Making an Informed Decision on Purchasing</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/complete-guide-for-recovering-messages-files-on-nubia-flip-5g-by-fonelab-android-recover-messages/"><u>Complete guide for recovering messages files on Nubia Flip 5G</u></a></li>
<li><a href="https://youtube-web.techidaily.com/vate-creativity-best-video-concepts-for-viewers/"><u>Cultivate Creativity Best Video Concepts for Viewers</u></a></li>
<li><a href="https://win-info.techidaily.com/from-humor-to-harsh-facts-how-microsofts-team-jokes-reflected-deeper-challenges-insights-from-zdnet/"><u>From Humor to Harsh Facts: How Microsoft’s Team Jokes Reflected Deeper Challenges - Insights From ZDNet</u></a></li>
<li><a href="https://fake-location.techidaily.com/how-to-find-ispoofer-pro-activation-key-on-oppo-find-n3-flip-drfone-by-drfone-virtual-android/"><u>How to Find iSpoofer Pro Activation Key On Oppo Find N3 Flip? | Dr.fone</u></a></li>
<li><a href="https://win-info.techidaily.com/ifixit-amazed-by-microsofts-easy-to-repair-latest-laptop-line-setting-a-new-benchmark-for-competitors-including-apple/"><u>IFixit Amazed by Microsoft's Easy-to-Repair Latest Laptop Line: Setting a New Benchmark for Competitors Including Apple</u></a></li>
<li><a href="https://win-info.techidaily.com/mastering-excel-formula-writing-with-chatgpt-a-comprehensive-guide/"><u>Mastering Excel Formula Writing with ChatGPT: A Comprehensive Guide</u></a></li>
<li><a href="https://win-info.techidaily.com/microsofts-50m-strategic-investment-boosts-lanzajets-green-aviation-fuels-for-eco-friendly-data-centers/"><u>Microsoft's $50M Strategic Investment Boosts LanzaJet’s Green Aviation Fuels for Eco-Friendly Data Centers</u></a></li>
<li><a href="https://win11.techidaily.com/solutions-for-disabled-taskbar-icon-clicks/"><u>Solutions for Disabled Taskbar Icon Clicks</u></a></li>
<li><a href="https://buynow-marvelous.techidaily.com/unveiling-the-powerful-tech-in-asus-ax6000-rt-ax88u-an-in-depth-look-at-a-cutting-edge-smart-wi-fi-grower/"><u>Unveiling the Powerful Tech in Asus AX6000 (RT-AX88U): An In-Depth Look at a Cutting-Edge Smart Wi-Fi Grower</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/virtual-vulnerabilities-love-by-algorithm/"><u>Virtual Vulnerabilities: Love by Algorithm</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1938716/19272" target="_top" id="1938716">
  <img src="//a.impactradius-go.com/display-ad/19272-1938716" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1938716/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

