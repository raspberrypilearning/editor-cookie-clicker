## Make the clicker bounce

Give your main sprite a bit of life when it is clicked.

<h2 class="c-project-heading--explainer">What you need to do</h2>

![The example project's pizza sprite.](images/pizza.png)

Add blocks to make the sprite grow, wait for a moment, and shrink back to its starting size.

```blocks3
when this sprite clicked
start sound (Tennis Hit v)
change [pizzas v] by (1)
+change size by (10)
+wait (0.05) seconds
+change size by (-10)
```

## Tip

**Visual feedback** shows the player that an action worked. The bounce makes every click feel real, even before the player checks the score.

## Now run your code

Click your sprite. It pops bigger for a moment with every click.
