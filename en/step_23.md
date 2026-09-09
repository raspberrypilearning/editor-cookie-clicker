## Initialize the granny variables

Set the granny count and price before the sprite can be clicked or shown.

<h2 class="c-project-heading--explainer">What you need to do</h2>

![Selecting the Stage, to the right of the sprite list.](images/select-stage.png)

Click the `Stage`{:class="block3looks"} and add both values to the green-flag script.

The second helper starts at `100` pizzas because it works five times faster than the first helper.

```blocks3
when green flag clicked
set [pizzas v] to (0)
set [pizzas per click v] to (1)
set [helpers v] to (0)
set [helper price v] to (50)
+set [grannies v] to (0)
+set [granny price v] to (100)
update pizzas per second :: custom
forever
wait (1) seconds
change [pizzas v] by (pizzas per second)
end
```

## Now run your code

Click the green flag. The new readouts show `grannies 0` and `granny price 100`.

The second helper cannot be free when you add its scripts next.
