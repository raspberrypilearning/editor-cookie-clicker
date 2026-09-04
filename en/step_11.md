## Buy the cutter

Let the player click the cutter to upgrade their clicks.

![The example project's cutter.](images/cutter.png)

Add the `Tada`{:class="block3sound"} sound to your equipment sprite.

Then add a click script that checks the cutter is still unbought and affordable. Buying it spends 25 pizzas, adds `1` to the multiplier, and switches to the bought costume.

```blocks3
when this sprite clicked
if <<(costume [number v]) = (1)> and <(pizzas) > (24)>> then
start sound (Tada v)
change [pizzas v] by (-25)
change [pizzas per click v] by (1)
next costume
end
```

The costume check means the plain cutter can be bought once, but its green-tick costume cannot be bought again.

## Now run your code

Reach 25 pizzas, then click the cutter. The cost is deducted and every click is now worth 2 pizzas.

## Tip

Game developers often build and test one working **prototype** first. Fixing the cutter before copying its scripts makes problems easier to find.
