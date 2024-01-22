Mask  active phaser:
Absolute preset: 65
Relative only, activated from a preset: 66
relative only, hard value in programmer: 64
First two bits are absolute, then relative respectively
Add a line to phaser and it goes to 83, activate bit 5

If I make a phaser with two steps and no phase information, I get 65 again (first bit)
If I activate phase information, Then it activates bit 6

If I make a two step phaser, one with absolute preset and one with relative preset, it comes up as 65. If I add phase information it comes up as 81, which is activating bit 5, but without bit 2.

Here's what I'm getting for a bit layout
```
<Unk><Prog Active><Phase><Speed><Delay><Fade><Rel><Abs>
```

The same things are consistent with the same kind of values applied in MATricks. Worth noting that these bits are only active for abs and relative if they're coming from  a preset, not hard programmer values. 