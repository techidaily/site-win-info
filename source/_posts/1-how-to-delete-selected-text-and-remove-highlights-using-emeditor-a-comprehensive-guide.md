---
title: 1. How to Delete Selected Text and Remove Highlights Using EmEditor - A Comprehensive Guide
date: 2024-10-05T16:22:05.674Z
updated: 2024-10-08T16:03:55.389Z
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
<li><a href="https://win-info.techidaily.com/elite-guide-to-purchasing-windows-laptops-comprehensive-reviews-and-expert-opinions-zdnet/"><u>Elite Guide to Purchasing Windows Laptops: Comprehensive Reviews & Expert Opinions | ZDNet</u></a></li>
<li><a href="https://win-info.techidaily.com/enhancing-ai-powered-music-creation-with-the-latest-upgrades-on-github-copilot-techzdnet/"><u>Enhancing AI-Powered Music Creation with the Latest Upgrades on GitHub Copilot | TechZDNet</u></a></li>
<li><a href="https://buynow-info.techidaily.com/evaluating-nhl-19-for-gamers-exciting-interactive-play-breakdown/"><u>Evaluating NHL 19 for Gamers: Exciting Interactive Play Breakdown</u></a></li>
<li><a href="https://win-info.techidaily.com/exploring-the-microsoft-surface-laptop-n-a-closer-look-at-classic-features-and-new-enhancements-insights-from-zdnet/"><u>Exploring the Microsoft Surface Laptop N: A Closer Look at Classic Features & New Enhancements | Insights From ZDNET</u></a></li>
<li><a href="https://win-info.techidaily.com/exploring-user-preferences-the-top-trending-internet-browsers/"><u>Exploring User Preferences: The Top Trending Internet Browsers</u></a></li>
<li><a href="https://windows11.techidaily.com/fixing-non-initialized-disks-a-windows-guide/"><u>Fixing Non-Initialized Disks: A Windows Guide</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/gionee-f3-pro-messages-recovery-recover-deleted-messages-from-gionee-f3-pro-by-fonelab-android-recover-messages/"><u>Gionee F3 Pro Messages Recovery - Recover Deleted Messages from Gionee F3 Pro</u></a></li>
<li><a href="https://win-info.techidaily.com/how-crowdstrike-triggered-widespread-system-failures-across-key-sectors-unraveling-the-incidents-impact-on-airports-and-finance/"><u>How CrowdStrike Triggered Widespread System Failures Across Key Sectors: Unraveling the Incident's Impact on Airports & Finance</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/in-2024-fb-video-retrieval-the-top-5-software-compared/"><u>In 2024, FB Video Retrieval The Top 5 Software Compared</u></a></li>
<li><a href="https://pokemon-go-android.techidaily.com/in-2024-how-and-where-to-find-a-shiny-stone-pokemon-for-honor-x9b-drfone-by-drfone-virtual-android/"><u>In 2024, How and Where to Find a Shiny Stone Pokémon For Honor X9b? | Dr.fone</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/mastering-the-art-of-data-visualization-for-effective-communication-for-2024/"><u>Mastering the Art of Data Visualization for Effective Communication for 2024</u></a></li>
<li><a href="https://win-info.techidaily.com/microsoft-faces-major-challenges-with-windows-10-just-one-year-remaining-to-find-solutions-technewszdnet/"><u>Microsoft Faces Major Challenges with Windows 10: Just One Year Remaining to Find Solutions | TechNewsZDNet</u></a></li>
<li><a href="https://win-info.techidaily.com/microsoft-raises-the-repairability-game-with-new-laptops-leaving-ifixit-impressed-and-rivals-like-apple-under-pressure-zdnet/"><u>Microsoft Raises the Repairability Game with New Laptops, Leaving iFixit Impressed and Rivals Like Apple Under Pressure | ZDNET</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/periscope-stars-in-snapchat-highlights-for-2024/"><u>Periscope Stars in Snapchat Highlights for 2024</u></a></li>
<li><a href="https://article-helps.techidaily.com/the-common-day-duel-claude-against-the-ai-giants/"><u>The Common Day Duel: Claude Against the AI Giants</u></a></li>
<li><a href="https://vp-tips.techidaily.com/transforming-media-captions-the-creme-de-la-creme-of-top-online-editors-for-2024/"><u>Transforming Media Captions The Crème De La Créme of Top Online Editors for 2024</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135418/19272" target="_top" id="2135418">
  <img src="//a.impactradius-go.com/display-ad/19272-2135418" border="0" alt="https://techidaily.com" width="468" height="60"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135418/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

