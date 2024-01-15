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


Workflow thinking:

Create an all pool that's designated for recipes
Create window separation for each song like I do with others. (may not be necessary)
For each song macro, set the current pointer to that point in the recipe all pool.


## Cat west video

Potentially old info, reading more
Recipes can't reference themselves, So org isimportant
Edit setting- add group, add preset/value
Assign syntax- assign-touch group/value, touch column for recipe
Last column is for matricks. You can manually input values or select a matricks pool object. Pool items will show up with angle brackets.


When do we need to cook- when you first create a recipe, the console will cook automatically for the first time. If you change the ingredients of a recipe, you may need to cook. If you change the matricks or group value items you'll need to cook

DANGER:
If you change the group in a recipe preset, and it's referenced in a cue, the fixtures used in that cue will NOT update. It'll leave hard values from what was there before in the track sheet. 

Maybe this means  I'll need to use cue recipes and not presets? That could destroy the workflow and mean that I'd need to recook EVERY CUE in a show. That sucks. 






I might have luck with the turn into recipe AND take selection commands

Maybe the right idea is actually to move everything to cue recipes, with groups