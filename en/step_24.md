## Make grannies worth more

Each granny should be worth `5` pizzas a second.

![Selecting the Stage, to the right of the sprite list.](images/select-stage.png)

On the `Stage`{:class="block3looks"}, update the `update pizzas per second`{:class="block3custom"} definition.

```blocks3
define update pizzas per second
+set [pizzas per second v] to (((chefs) * (1)) + ((grannies) * (5)))
```

Your grannies still start at zero.

You'll give them a price on the green flag next.
