## Count both helpers

Make each granny add five pizzas per second, then test the complete helper system.

<h2 class="c-project-heading--explainer">What you need to do</h2>

![Selecting the Stage, to the right of the sprite list.](images/select-stage.png)

On the `Stage`{:class="block3looks"}, update the `update pizzas per second`{:class="block3custom"} definition.

The first helpers each add one pizza per second. Multiply only `grannies`{:class="block3variables"} by `5`.

```blocks3
define update pizzas per second
+set [pizzas per second v] to ((helpers) + ((grannies) * (5)))
```

## Tip

Choosing costs and rewards so each upgrade feels worthwhile is called **game balancing**.

You now have the clicker's **core loop**: click, earn, buy upgrades, and earn faster.

## Now run your code

Click the green flag. Check that both helper counts start at `0`, the first helper costs `50`, the granny costs `100`, and `pizzas per second`{:class="block3variables"} starts at `0`.

Earn 50 pizzas and buy the first helper. Its count becomes `1`, its next price becomes `58`, and the earning rate becomes `1`.

Earn 100 pizzas and buy the granny. Its count becomes `1`, its next price becomes `115`, and `pizzas per second`{:class="block3variables"} becomes `6`.

Stop clicking and check that the score rises by six each second.
