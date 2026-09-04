## Make every click worth more

Set up the number that decides how much each click is worth.

![Selecting the Stage, to the right of the sprite list.](images/select-stage.png)

## Step 1

Make a variable called `pizzas per click`{:class="block3variables"}.

If you gave your score a different name, use a matching name such as `coins per click`{:class="block3variables"}.

## Step 2

Click the `Stage`{:class="block3looks"} and set the new variable to `1` on the green flag, so each click always adds at least one.

```blocks3
when green flag clicked
set [pizzas v] to (0)
+set [pizzas per click v] to (1)
```

## Tip

All the changing information a game remembers, like scores, prices, and upgrades, is called the **game state**.

Nothing changes yet. You'll put this number to work next.
