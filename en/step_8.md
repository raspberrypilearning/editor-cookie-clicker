## Spend the multiplier

Make each click use your new number instead of a fixed `1`.

![the pizza sprite](images/pizza.png)

On your pizza sprite, change the click script to add `pizzas per click`{:class="block3variables"} instead.

```blocks3
when this sprite clicked
start sound (Tennis Hit v)
+change [pizzas v] by (pizzas per click)
change size by (10)
wait (0.05) seconds
change size by (-10)
```

Nothing changes yet, because `pizzas per click`{:class="block3variables"} is still `1`.

The equipment you add next will raise it.
