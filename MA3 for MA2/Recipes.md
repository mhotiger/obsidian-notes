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
