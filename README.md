# tdjr_rt_complete  
<img src="https://github.com/tillmanjr/tdjr_rt_complete/raw/master/tdjr_rt_complete_mini.png" align="right" />  
A customization of the Ancient One's custom output *Character Sheet* for <a href="http://www.wolflair.com/index.php?context=hero_lab">Hero Lab</a>  
  
It adds a new control panel section for quick navigation to specific sections within the character sheet.  
To see it in action, scroll to the bottom of this readme.
  
## To use:
1. Click the button for the section you'd like to see.  
2. The related section will scroll immediately into view and be briefly hightlighted.  

#### Use Notes   
* Highlighting is a a 3s pulse animation. It could use some section specific tweaking or a better form of highlighting.  
  **Feature Update Completed**. See below _May 14, 2019 Update_
* Navigating to *Spec Abilities* require the character sheet override *Show Feat/Ability Descriptions* to be enabled.  
   If the override is not enabled when *Spec Abilities* is selected the override will be automatically enabled then the section will be scrolled into view  	
 to be selected.  
A similar concern may also apply to Spells - *Spell navigation is barely tested*

## To install:
1. Navigate to where Hero Lab stores its custom output on your computer.
_Typically here:_ C:\ProgramData\Hero Lab\customoutput\pathfinder  
2. Create a new directory named: tdjr_rt_complete  
3. Copy the two files into the newly created directory.  
* output.xml
* tdjr_rt_complete.xsl
4. Open Hero Lab _(no need to reload Hero Lab if it is already running_  
5. Load your character/portfolio  
6. File | Save Custom Output | Tillman's ...
7. Enjoy easier navigation of Ancient One's excellent Character Sheet
  
### Update May 13, 2019
Revamped the highlight feature for the requested section.

During a long scroll it can take a few moments for the eyes to settle and find the requested section.
So, the requested section (the target) was enhanced by physically pulsing its size on scroll to.
The physical size pulse didn't work so well along with the effect needed to be delay until the target was at least on screen.

1. Removed the size pulse on scroll.
2. Now starts scrolls on click 
3. Once the target section becomes visible on screen (detected using intersectionObserver) the target background color is set to the HeroLab yellow/khaki color with mid opacity with a 1s transition which fades it back to the original white.

**Result**: The indicator is much more useful indicator and sizing side effects have been eliminated
Note: repo sample images have not been updated to show this change
  
  
  
![screenshot of new control panel](
        https://github.com/tillmanjr/tdjr_rt_complete/raw/master/tdjr_rt_complete_screenshot.png
      )
      
### New control panel in action
![animated gif of new control panel in action](
        https://github.com/tillmanjr/tdjr_rt_complete/raw/master/tdjr_rt_complete_see_it_in_action.gif
        )
      
