## Win only when fully equipped

Make winning need all the upgrades, not just a high score.

![the pizza sprite](images/pizza.png)

On your pizza, update the `wait until`{:class="block3control"} so the player needs a high score **and** all the equipment (which lands `pizzas per click`{:class="block3variables"} on `24`).

```blocks3
when green flag clicked
set drag mode [not draggable v]
+wait until <<(pizzas) > (10000)> and <(pizzas per click) = (24)>>
start sound (Win v)
say [You Win!] for (2) seconds
stop [all v]
```

## Now run your code

Buy all three pieces of equipment and pass 10,000 pizzas.

The win message only appears once your shop is fully kitted out.
