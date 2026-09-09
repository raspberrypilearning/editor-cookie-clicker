## Win only when fully equipped

Make winning depend on buying every upgrade, not just reaching a high score.

<h2 class="c-project-heading--explainer">What you need to do</h2>

![The example project's pizza sprite.](images/pizza.png)

On your main clicker sprite, update the `wait until`{:class="block3control"} condition.

The player now needs more than 10,000 pizzas **and** a `pizzas per click`{:class="block3variables"} value of `24`.

The multiplier starts at `1`. The guarded purchases add `1`, `4`, and `18`, so it reaches `24` only after all three pieces have been bought — no matter which order the player buys them in.

```blocks3
when green flag clicked
set drag mode [not draggable v]
+wait until <<(pizzas) > (10000)> and <(pizzas per click) = (24)>>
start sound (Win v)
say [You Win!] for (2) seconds
stop [all v]
```

## Now run your code

Buy all three pieces of equipment and pass 10,000 pizzas. The win message only appears once your shop is fully equipped.
