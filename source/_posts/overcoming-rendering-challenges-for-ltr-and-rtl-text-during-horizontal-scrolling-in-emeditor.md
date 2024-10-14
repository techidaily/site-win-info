---
title: Overcoming Rendering Challenges for LTR and RTL Text During Horizontal Scrolling in EmEditor
date: 2024-10-07T20:54:09.882Z
updated: 2024-10-14T08:05:08.802Z
tags:
  - product
categories:
  - emeditor
thumbnail: https://thmb.techidaily.com/abfdd510a65bfb2974ae748187d91d88c050827e452b20253ad5c2d81a1eb51a.jpg
---

## Overcoming Rendering Challenges for LTR and RTL Text During Horizontal Scrolling in EmEditor

Viewing 3 posts - 1 through 3 (of 3 total)

* Author  
Posts
* April 11, 2016 at 12:54 pm [#20699](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/c7b1aac02d35a121a2acb8d8c9970c9b?s=80&d=identicon&r=g)Meir](https://www.emeditor.com/forums/users/meir/ "View Meir's profile")  
Participant  
Hi Yutaka,  
EmEditor is very good at displaying TSV texts. I have lots of these files and many of them have very long lines that leave large parts of the line off-screen. When I scroll horizontally to reveal these off-screen text, the display is badly rendered and garbled. Clicking anywhere in the window causes EE to re-render the display correctly. This is rather annoying.  
Yutaka, please read on. I am not suggesting to make EE a BiDi editor, (although this would make me rather happy :-)). I suspect that this is a small rendering problem but still…!  
I will send you screen shots of both the garbled display and how it should look. I will also send you a file that demonstrate the problem.  
Regards  
 Meir  
April 12, 2016 at 3:00 pm [#20709](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a0a6377144ed3636f985d87303f65ed2?s=80&d=identicon&r=g)Yutaka Emura](https://www.emeditor.com/forums/users/yemura/ "View Yutaka Emura's profile")  
Keymaster  
Hello Meir,  
You can write a macro (it can be a dummy macro, for example just one comment line)  
`//`  
and then associate to the “Scrolled” event. (Macros menu > Customize > select the macro name you created, click “Runs at Events”, click “Events…” button, and check “Scrolled”, and select Delay Time 0.  
When a macro is finished running, EmEditor automatically redraws the whole window.  
Thanks!  
April 13, 2016 at 1:50 am [#20713](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/c7b1aac02d35a121a2acb8d8c9970c9b?s=80&d=identicon&r=g)Meir](https://www.emeditor.com/forums/users/meir/ "View Meir's profile")  
Participant  
Thanks Yutaka!  
Works like a charm! Proves, as though a proff was required, how little I know this tool that I use for six-plus years… I repeat my “Tip-of-the-Day” suggestion.
* Author  
Posts

Viewing 3 posts - 1 through 3 (of 3 total)

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
<li><a href="https://win-info.techidaily.com/1-how-to-delete-selected-text-and-remove-highlights-using-emeditor-a-comprehensive-guide/"><u>1. How to Delete Selected Text and Remove Highlights Using EmEditor - A Comprehensive Guide</u></a></li>
<li><a href="https://win-info.techidaily.com/2-seamless-continuation-in-text-editing-with-emeditor-tips-for-restarting-nr-on-an-active-file/"><u>2. Seamless Continuation in Text Editing with EmEditor - Tips for Restarting 'Nr' On an Active File</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/best-motorola-moto-g34-5g-pattern-lock-removal-tools-remove-android-pattern-lock-without-losing-data-by-drfone-android/"><u>Best Motorola Moto G34 5G Pattern Lock Removal Tools Remove Android Pattern Lock Without Losing Data</u></a></li>
<li><a href="https://win-info.techidaily.com/creating-your-first-macro-with-emeditor-tips-and-tricks-for-text-editing-automation/"><u>Creating Your First Macro with EmEditor: Tips and Tricks for Text Editing Automation</u></a></li>
<li><a href="https://win-info.techidaily.com/emeditor-text-editor-fixing-projectsdll-error-and-preventing-application-crashes/"><u>EmEditor Text Editor: Fixing Projects.dll Error and Preventing Application Crashes</u></a></li>
<li><a href="https://win-info.techidaily.com/enhance-your-editing-with-emeditor-exploring-the-clipboard-monitor-capability/"><u>Enhance Your Editing with EmEditor - Exploring the Clipboard Monitor Capability</u></a></li>
<li><a href="https://hardware-tips.techidaily.com/expert-insights-on-computing-from-toms-hardware-hub/"><u>Expert Insights on Computing From Tom's Hardware Hub</u></a></li>
<li><a href="https://techno-recovery.techidaily.com/finding-the-right-pace-whats-ideal-for-your-pc/"><u>Finding the Right Pace: What's Ideal for Your PC?</u></a></li>
<li><a href="https://win-info.techidaily.com/how-to-fix-outline-text-issues-in-emeditor-a-comprehensive-guide/"><u>How to Fix 'Outline Text' Issues in EmEditor: A Comprehensive Guide</u></a></li>
<li><a href="https://win-info.techidaily.com/line-sorting-feature-in-emeditor-arrange-based-on-line-size-for-improved-readability/"><u>Line Sorting Feature in EmEditor: Arrange Based on Line Size for Improved Readability</u></a></li>
<li><a href="https://buynow-tips.techidaily.com/samsung-galaxy-a20-analysis-remains-an-excellent-affordable-phone/"><u>Samsung Galaxy A20 Analysis: Remains an Excellent Affordable Phone</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/skyrocketing-channels-essential-narrative-methods-for-2024/"><u>Skyrocketing Channels Essential Narrative Methods for 2024</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/the-art-of-producing-high-impact-slack-channels/"><u>The Art of Producing High-Impact Slack Channels</u></a></li>
<li><a href="https://android-transfer.techidaily.com/two-ways-to-sync-contacts-from-htc-u23-to-gmail-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>Two Ways to Sync Contacts from HTC U23 to Gmail | Dr.fone</u></a></li>
<li><a href="https://windows11.techidaily.com/unveiling-the-cause-of-winmedia-error/"><u>Unveiling the Cause of WinMedia Error</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2130889/7443" target="_top" id="2130889">
  <img src="//a.impactradius-go.com/display-ad/7443-2130889" border="0" alt="https://techidaily.com" width="600" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2130889/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

