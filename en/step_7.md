## Make every click worth more

Set up the number that decides how much each click is worth.

![Selecting the Stage, to the right of the sprite list.](images/select-stage.png)

## Step 1

Make a variable called `pizzas per click`{:class="block3variables"}.

This is how many pizzas one click makes.

## Step 2

Click the `Stage`{:class="block3looks"} and set it to `1` on the green flag, so a click always makes at least one pizza.

```blocks3
when green flag clicked
set [pizzas v] to (0)
+set [pizzas per click v] to (1)
```

## Tip

All the changing information a game remembers, like scores, prices, and upgrades, is called the **game state**.

Nothing changes in the game yet.

You'll put this number to work on your pizza next.
