
MA Grid interpolation concept- MAGIC

aligning  values across a range of fixtures. A way to make a gradient across fixtures.
Stpes:
1. select two fixtures
2. select one color on one fixture
3. another on the second fixture
4. select both fixtures
5. select at- then at magic
6. store preset
We'll know its a magic preset because of the hat icon.
We can apply that to any other group of fixtures, and those values will be spread and interpolated across the selection of fixtures on the x axis.

We could recreate the same thing with align wheels, but this works for other selections

It has a selective s, but works kind of more like global. It works for any of the same fixture type.
**If you use a magic preset straight up, it'll put hard values into the cue sheet.** 

This can work in x and y directions, it all depencds on the selection grid setup when you store the magic preset. 

You can store this an an embedded so that it will reference the original presets. 
If we go back and edit the color presets the magic is referencing, the magic updates, but it doesn't update  any cues that use the magic preset.

You can use a recipe in a cue to reference a magic preset, and then it's updateable via "cooking" the recipe preset