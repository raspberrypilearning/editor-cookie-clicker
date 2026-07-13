## Give the grannies a price

Set the granny's starting values so the game runs from the first click.

![Selecting the Stage, to the right of the sprite list.](images/select-stage.png)

You're still working on the `Stage`{:class="block3looks"}.

Give the new variables their starting values on the green flag.

A granny starts at `100` pizzas, pricier than a chef because she works harder.

```blocks3
when green flag clicked
set [pizzas v] to (0)
set [pizzas per click v] to (1)
set [chefs v] to (0)
set [chef price v] to (15)
+set [grannies v] to (0)
+set [granny price v] to (100)
update pizzas per second
forever
wait (1) seconds
change [pizzas v] by (pizzas per second)
end
```

## Now run your code

Buy chefs, then save for a granny and watch your pizzas-per-second jump.

You now have a full endless clicker: clicks, upgrades, and helpers all working together.
