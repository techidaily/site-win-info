---
title: "Creating Your First Macro with EmEditor: Tips and Tricks for Text Editing Automation"
date: 2024-10-07T03:14:43.875Z
updated: 2024-10-13T23:10:39.882Z
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
<li><a href="https://visual-screen-recording.techidaily.com/new-2024-approved-expert-advice-on-screen-casting-in-google-meet/"><u>[New] 2024 Approved Expert Advice on Screen Casting in Google Meet</u></a></li>
<li><a href="https://win-info.techidaily.com/1-how-to-delete-selected-text-and-remove-highlights-using-emeditor-a-comprehensive-guide/"><u>1. How to Delete Selected Text and Remove Highlights Using EmEditor - A Comprehensive Guide</u></a></li>
<li><a href="https://win-info.techidaily.com/2-seamless-continuation-in-text-editing-with-emeditor-tips-for-restarting-nr-on-an-active-file/"><u>2. Seamless Continuation in Text Editing with EmEditor - Tips for Restarting 'Nr' On an Active File</u></a></li>
<li><a href="https://fox-glue.techidaily.com/2024-approved-why-are-my-instagram-photos-flipped-seeking-answers/"><u>2024 Approved Why Are My Instagram Photos Flipped? Seeking Answers</u></a></li>
<li><a href="https://solve-popular.techidaily.com/efficiently-managing-insurance-claims-with-ecclesia-the-abbyy-integration/"><u>Efficiently Managing Insurance Claims with Ecclesia: The ABBYY Integration</u></a></li>
<li><a href="https://win-info.techidaily.com/emeditor-text-editor-fixing-projectsdll-error-and-preventing-application-crashes/"><u>EmEditor Text Editor: Fixing Projects.dll Error and Preventing Application Crashes</u></a></li>
<li><a href="https://win-info.techidaily.com/enhance-your-editing-with-emeditor-exploring-the-clipboard-monitor-capability/"><u>Enhance Your Editing with EmEditor - Exploring the Clipboard Monitor Capability</u></a></li>
<li><a href="https://change-location.techidaily.com/in-2024-3utools-virtual-location-not-working-on-honor-magic5-ultimate-fix-now-drfone-by-drfone-virtual-android/"><u>In 2024, 3uTools Virtual Location Not Working On Honor Magic5 Ultimate? Fix Now | Dr.fone</u></a></li>
<li><a href="https://extra-tips.techidaily.com/pro-tips-for-effective-use-of-supplemental-film-sequences-b-roll/"><u>Pro Tips for Effective Use of Supplemental Film Sequences (B-Roll)</u></a></li>
<li><a href="https://win-info.techidaily.com/professional-text-editing-software-emeditor-pro-version-900-beta-update/"><u>Professional Text Editing Software - EmEditor Pro Version 9.00 Beta Update</u></a></li>
<li><a href="https://buynow-info.techidaily.com/stateless-address-autoconfiguration-in-ipv6-can-introduce-privacy-and-prediction-issues-if-additional-security-measures-are-not-applied/"><u>Stateless Address Autoconfiguration in IPv6 Can Introduce Privacy and Prediction Issues if Additional Security Measures Are Not Applied</u></a></li>
<li><a href="https://buynow-info.techidaily.com/1722701037883-unbeatable-prime-day-discounts-sweet-apple-savings-await/"><u>Unbeatable Prime Day Discounts: Sweet Apple Savings Await!</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2144278/7443" target="_top" id="2144278">
  <img src="//a.impactradius-go.com/display-ad/7443-2144278" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2144278/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

