## Set up winning

Lock the clicker in place, then decide when the player has won.

![The example project's pizza sprite.](images/pizza.png)

## Step 1

Add the `Win`{:class="block3sound"} sound to your clicker sprite.

Start a new script. On the green flag, set the sprite to `not draggable`{:class="block3sensing"} so the player clicks it instead of accidentally dragging it.

```blocks3
when green flag clicked
set drag mode [not draggable v]
```

## Step 2

Add the **win condition** to the same script. It waits until the score is high enough, then celebrates.

```blocks3
when green flag clicked
set drag mode [not draggable v]
+wait until <(pizzas) > (10000)>
+start sound (Win v)
+say [You Win!] for (2) seconds
+stop [all v]
```

## Tip

A **win condition** is the rule that decides when a player has completed or won a game.

You will add faster ways to reach 10,000 as you build the rest of the game.
