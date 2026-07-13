## Buy a chef

Let the player click the chef to hire one.

![The pizza shop's robot chef.](images/chef.png)

You're still working on the `Chef`{:class="block3looks"} sprite.

Clicking it spends pizzas, hires one helper, and raises the price for next time.

```blocks3
when this sprite clicked
start sound (Clang v)
change [pizzas v] by ((0) - (chef price))
change [chefs v] by (1)
set [chef price v] to (round ((chef price) * (1.15)))
```

Multiplying the price by `1.15` makes each helper cost about 15% more than the last.

That steady climb is the trick behind every endless clicker.

## Tip

A **progression curve** controls how quickly a game gets harder, faster, or more expensive as the player improves.

The chef won't show up yet.

You'll make it appear when it's affordable next.
