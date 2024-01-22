https://www.youtube.com/watch?v=L9-CSR_RP6Y

Create a new preset and edit
Create recipe
assign group x![[Pasted image 20240113183942.png]]

Flowchart for recipe data output decision. 

Recipes can be stored in presets or in a cue part directly. I think it'll be wise to always store in a cue part, putting them in the cues sounds like a good way for things to not get updated properly. 

Recipe presets can:
- create recipe presets for groups, and reference other presets in the show so fixture selection is flexible. 
- create a template preset with ranged values that can be applied to variable selections of fixtures. 

There are multiple parts of a recipe preset:
References:
 - the fixture selection, can either be a group number or from the programmer, which shows as \<recipe>
 - values referenced form the recipe line. Could be a preset value or the programmer
 - MATricks: ref to existing MAT pool object, overrrides the matricks section of the actual recipe. 

Layers: Fade, Delay, Speed, Phase


Creating a recipe preset:
any preset needs to be turned into a recipe. You can turn into a recipe from an existing preset with values already there, or create a new blank recipe. 


[[notes-repo/ma3 for ma2/Recipe Workflow]]

Notes on recipes with instances:

Store instances for your recipes to work. 
Add new fixtures  with instances, and store in to a group used in a recipe.
You need to select the fixtures AND the instances and store them into the group for the recipes to continue working. You can easily select all instances by selecting the fixtures and hitting the down key. 


Can recipes track/cueonly?



I might have luck with the turn into recipe AND take selection commands

Maybe the right idea is actually to move everything to cue recipes, with groups