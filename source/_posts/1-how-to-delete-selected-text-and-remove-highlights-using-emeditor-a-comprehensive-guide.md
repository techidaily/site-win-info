---
title: 1. How to Delete Selected Text and Remove Highlights Using EmEditor - A Comprehensive Guide
date: 2024-10-09T08:55:16.362Z
updated: 2024-10-13T16:16:57.892Z
tags:
  - product
categories:
  - emeditor
thumbnail: https://thmb.techidaily.com/8f59b16f9ed7024a23cc6f18f766904b6f418e4c5b8df6a84d93cf668a943550.jpg
---

## 1. How to Delete Selected Text and Remove Highlights Using EmEditor - A Comprehensive Guide

July 27, 2010 at 11:33 pm [#8804](https://tools.techidaily.com/emeditor/products/) 

[![](https://secure.gravatar.com/avatar/c095e276d7d1f5ed27f91bf623e4e445?s=80&d=identicon&r=g)CrashNBurn](https://www.emeditor.com/forums/users/CrashNBurn/ "View CrashNBurn's profile")

Member

I didn’t want to disable the Find Highlight.   
 My request was to to automatically clear the Find Highlight when the Find Dialog was closed — if a checkbox on the find dialog was checked: \[x\] Clear Highlights.

 I solved it with AutoHotKey. The original AHK solution was Kludgy and didn’t work consistently.

 Perhaps someone else will find some use for it.  
 Fixed **clean** code:

;;  

	;;  Script: EE_AutoClearFindHighlight.ahk  

	;;  Author: MwM - Crash&Burn, 2010  

	;;  Usage::   

	;;    Automatically clear the Find Highlight when EmEditor's  

	;;    Find Dialog is closed with the [Close] Button.  

	;;  

	;;    Does not clear the Find Highlight if ESC, or the   

	;;    Find Dialog's TitleBar [X] is used, nor if a modifier  

	;;    key is held down when clicking [Close] (i.e. Shift)  

	;;  

	  #SingleInstance, Force   

	  #NoEnv  

	SetBatchLInes, -1  
	  

	#ifWinActive, Find ahk_class #32770  

	  ~LButton::  

	; $ESC::  

	    aParent := DllCall("GetParent", UInt, WinExist("A"))  

	    aParent := ((!aParent) ? WinExist("A") : aParent)  

	    WinGetClass, aClass, ahk_id \%aParent\%   

	    if(aClass <> "EmEditorMainFrame3")  

	      return  

	    if(A_ThisHotKey == "LButton")  

	      MouseGetPos, ,, aFind, aControl  

	      if(aControl <> "Button16")  

	        return  

	      KeyWait, LButton  

	      Sleep, 50  

	      ifWinExist, ahk_id \%aFind\%  

	        return  

	      WinWaitActive, ahk_class EmEditorMainFrame3  

	      Send, !{F3}  

	    ;; If one wanted the Find Highlight to clear on ESC  

	    ;; Remove comment block below, and uncomment ESC above.  

	    /*  

	     *  

	    else      

	    if(A_ThisHotKey == "$ESC")        ;;  Not clearing Find Highlight on ESC, atm  

	      Send, {ESC}  

	      Sleep, 50  

	      ifWinExist, ahk_id \%aFind\%  

	        return  

	      WinWaitActive, ahk_class EmEditorMainFrame3  

	      Send, !{F3}  

	     *  

	     */  

	  return  

	return

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
<li><a href="https://facebook-video-share.techidaily.com/new-top-15-youtube-portals-on-stocks-and-trades/"><u>[New] Top 15 YouTube Portals on Stocks & Trades</u></a></li>
<li><a href="https://win-info.techidaily.com/2-seamless-continuation-in-text-editing-with-emeditor-tips-for-restarting-nr-on-an-active-file/"><u>2. Seamless Continuation in Text Editing with EmEditor - Tips for Restarting 'Nr' On an Active File</u></a></li>
<li><a href="https://change-location.techidaily.com/9-mind-blowing-tricks-to-hatch-eggs-in-pokemon-go-without-walking-on-samsung-galaxy-z-fold-5-drfone-by-drfone-virtual-android/"><u>9 Mind-Blowing Tricks to Hatch Eggs in Pokemon Go Without Walking On Samsung Galaxy Z Fold 5 | Dr.fone</u></a></li>
<li><a href="https://location-fake.techidaily.com/a-detailed-guide-on-faking-your-location-in-mozilla-firefox-on-realme-c33-2023-drfone-by-drfone-virtual-android/"><u>A Detailed Guide on Faking Your Location in Mozilla Firefox On Realme C33 2023 | Dr.fone</u></a></li>
<li><a href="https://win-info.techidaily.com/creating-your-first-macro-with-emeditor-tips-and-tricks-for-text-editing-automation/"><u>Creating Your First Macro with EmEditor: Tips and Tricks for Text Editing Automation</u></a></li>
<li><a href="https://win-info.techidaily.com/emeditor-text-editor-fixing-projectsdll-error-and-preventing-application-crashes/"><u>EmEditor Text Editor: Fixing Projects.dll Error and Preventing Application Crashes</u></a></li>
<li><a href="https://win-info.techidaily.com/enhance-your-editing-with-emeditor-exploring-the-clipboard-monitor-capability/"><u>Enhance Your Editing with EmEditor - Exploring the Clipboard Monitor Capability</u></a></li>
<li><a href="https://tech-renaissance.techidaily.com/expert-tips-for-resolving-dll-errors-on-your-computer/"><u>Expert Tips for Resolving DLL Errors on Your Computer</u></a></li>
<li><a href="https://win-info.techidaily.com/how-to-fix-outline-text-issues-in-emeditor-a-comprehensive-guide/"><u>How to Fix 'Outline Text' Issues in EmEditor: A Comprehensive Guide</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/in-2024-read-this-guide-to-find-a-reliable-alternative-to-fake-gps-on-vivo-x100-drfone-by-drfone-virtual-android/"><u>In 2024, Read This Guide to Find a Reliable Alternative to Fake GPS On Vivo X100 | Dr.fone</u></a></li>
<li><a href="https://win-info.techidaily.com/introducing-emeditor-professional-v13-beta-6-enhanced-text-editing-experience/"><u>Introducing EmEditor Professional v13 Beta 6 - Enhanced Text Editing Experience.</u></a></li>
<li><a href="https://win-info.techidaily.com/line-sorting-feature-in-emeditor-arrange-based-on-line-size-for-improved-readability/"><u>Line Sorting Feature in EmEditor: Arrange Based on Line Size for Improved Readability</u></a></li>
<li><a href="https://extra-skills.techidaily.com/palette-playbook-the-filmmakers-guide-to-grading-for-2024/"><u>Palette Playbook The Filmmaker's Guide to Grading for 2024</u></a></li>
<li><a href="https://ai-voice.techidaily.com/pc-troubleshooting-guide-fix-ark-sanctuary-uber-wikis-constant-crash-issues-with-9-solutions/"><u>PC Troubleshooting Guide: Fix ARK: Sanctuary Über Wiki's Constant Crash Issues with 9 Solutions</u></a></li>
<li><a href="https://win-info.techidaily.com/potential-syntax-errors-no-worries-with-emeditor-your-reliable-text-editing-companion/"><u>Potential Syntax Errors? No Worries with EmEditor - Your Reliable Text Editing Companion!</u></a></li>
<li><a href="https://fake-location.techidaily.com/prank-your-friends-easy-ways-to-fake-and-share-google-maps-location-on-zte-nubia-z60-ultra-drfone-by-drfone-virtual-android/"><u>Prank Your Friends! Easy Ways to Fake and Share Google Maps Location On ZTE Nubia Z60 Ultra | Dr.fone</u></a></li>
<li><a href="https://win-info.techidaily.com/professional-text-editing-software-emeditor-pro-version-900-beta-update/"><u>Professional Text Editing Software - EmEditor Pro Version 9.00 Beta Update</u></a></li>
<li><a href="https://win-forum.techidaily.com/step-by-step-instructions-forcefully-erase-directories-in-windows-1011-using-professional-software/"><u>Step-by-Step Instructions: Forcefully Erase Directories in Windows 10/11 Using Professional Software</u></a></li>
<li><a href="https://win-bits.techidaily.com/understanding-the-wmv-video-file-format-a-comprehensive-guide/"><u>Understanding the WMV Video File Format: A Comprehensive Guide</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://laganoo.pxf.io/c/5597632/1484910/16446" target="_top" id="1484910">
  <img src="//a.impactradius-go.com/display-ad/16446-1484910" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://laganoo.pxf.io/i/5597632/1484910/16446" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

