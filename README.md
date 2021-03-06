#DC's Text Watch Deluxe
for Pebble Time Round smartwatch
* This is early version, with config.h rather than config.html for customizations
* <a href="https://drive.google.com/uc?export=download&id=0B3fA-FAkWLGNNmduNFI1aXdfLTA">Download compiled PBW here.</a>  (Default black color scheme, with O' displayed before single digits.)
* A <a href="https://github.com/wackyneighbor/DC_Text_Watch_Deluxe">more advanced version has been completed</a> and is now in <a href="https://apps.getpebble.com/en_US/application/56ab1cfe6ca919990000000e">the app store</a>.  This version enables the settings to be changed with <a href="http://wackyneighbor.github.io/DC_Text_Watch_Deluxe/config.html?SinglePrefixType=2&ColorScheme=1&BackgroundColor1=FFFFAA&TextLine1Color1=550055&TextLine2Color1=AA5500&TextLine3Color1=55AA00&TextDayColor1=FF0055&TextDateColor1=FF0055&TimeIndicatorColor1=55AA00&SunriseIndicatorColor1=AA5555&SunsetIndicatorColor1=AA5555&BackgroundColor2=000000&TextLine1Color2=AA5500&TextLine2Color2=AA5500&TextLine3Color2=AA5500&TextDayColor2=FFFF55&TextDateColor2=FFFFAA&TimeIndicatorColor2=FFAA00&SunriseIndicatorColor2=555500&SunsetIndicatorColor2=555500&BackgroundColor3=FF0000&TextLine1Color3=FFFF00&TextLine2Color3=FFFF55&TextLine3Color3=FFFF55&TextDayColor3=FFFFAA&TextDateColor3=FFFFAA&TimeIndicatorColor3=0000FF&SunriseIndicatorColor3=000000&SunsetIndicatorColor3=000000&return_to=https%3A//cloudpebble.net/ide/emulator/config%3F">a phone interface</a>.

<IMG SRC="https://cloud.githubusercontent.com/assets/16750280/12547778/0b42de68-c307-11e5-8310-744512919e15.gif" ALT="Time_Slide.gif" WIDTH=180 HEIGHT=180> --- <IMG SRC="https://cloud.githubusercontent.com/assets/16750280/12535171/8369a7b0-c22f-11e5-948e-c2df00479a72.gif" ALT="Time_Dial.gif" WIDTH=180 HEIGHT=180> --- <IMG SRC="https://cloud.githubusercontent.com/assets/16750280/12535172/89fc4934-c22f-11e5-90aa-ebca46483f1a.gif" ALT="Seasons.gif" WIDTH=180 HEIGHT=180>

<IMG SRC="https://cloud.githubusercontent.com/assets/16750280/12381789/d811c75a-bd45-11e5-9ceb-5e4b993f6339.png" ALT="Screenshot_1_0631_Summer.png" WIDTH=180 HEIGHT=180> --- <IMG SRC="https://cloud.githubusercontent.com/assets/16750280/12413112/4d01b632-be41-11e5-97d2-d9e387b711ea.png" ALT="surf.png" WIDTH=180 HEIGHT=180> --- <IMG SRC="https://cloud.githubusercontent.com/assets/16750280/12413115/4fe2e3ee-be41-11e5-9cf2-3ae9768d1a57.png" ALT="neapolitan.png" WIDTH=180 HEIGHT=180>

This is a variant of the "Sliding Time" text watch, with some significant enhancements:
*  Rather than "Twelve O'clock", it will say "Twelve Noon" or "Twelve Midnight".
*  The time display will always be centered vertically, whether it is 2 lines or 3 lines.  The transition is animated.
*  Single digit times can be prefixed with O' (same line) or with "Oh" (on an extra line), or with neither.  (Setting is in the config.h file.)
*  The day of the week is fully spelled out and shown in a large font below the time, with proper capitalization.
*  The date has the month abbreviated for space concerns at bottom of screen.  The proper ordinal suffix is used (e.g. "1st" rather than "1"). 
*  A subtle analog clock feature is incorporated.  A semicircle transverses the perimeter of the screen once a day, with midnight on the bottom and noon on top.
*  Two subtle dots along the perimeter identify the sunrise and sunset times.  These are computed on the watch, not looked up from a webservice.  To do this, it must determine location from phone.  Sunrise & sunset indicator dots will not appear on screen until this has been completed successful.  (Attempt will be made every minute until first success, with updates requested every hour afterwards.)  Time zone is recorded along with location, as well as if daylight savings time is in affect or not.  If either of these changes, but location has not been updated (e.g. cellular connection updated time, but GPS is switched off), sunrise & sunset should auto-correct to approximate local time.
*  Color of every element can be set individually in the config.h file.

See <a href="https://github.com/stars/wackyneighbor">projects I've starred</a> for various bits of code I've copied from.

By the way, I don't really know what I'm doing; I'm a mechanical systems designer by trade, not a coder.

<IMG SRC="http://imgs.xkcd.com/comics/code_quality.png" ALT="XKCD #1513 on Code Quality" WIDTH=740 HEIGHT=258>
