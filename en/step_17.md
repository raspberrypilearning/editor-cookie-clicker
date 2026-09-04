## Buy a helper

Let the player click the helper to hire one.

![The example project's robot chef.](images/chef.png)

## Step 1

Clicking the helper first checks the player can still afford it, then spends its current price and increases the number hired.

The `change`{:class="block3variables"} block needs a negative number to spend pizzas. `0 - helper price` turns the price into that negative number.

The affordability check also stops rapid repeat clicks from pushing the score below zero while the sprite is waiting to hide.

```blocks3
when this sprite clicked
if <(pizzas) > ((helper price) - (1))> then
start sound (Clang v)
change [pizzas v] by ((0) - (helper price))
change [helpers v] by (1)
end
```

## Step 2

Make the next helper cost about 15% more. `round`{:class="block3operators"} keeps the new price as a whole number.

```blocks3
when this sprite clicked
if <(pizzas) > ((helper price) - (1))> then
start sound (Clang v)
change [pizzas v] by ((0) - (helper price))
change [helpers v] by (1)
+set [helper price v] to (round ((helper price) * (1.15)))
end
```

## Tip

A **progression curve** controls how quickly a game gets harder, faster, or more expensive as the player improves.

The first helper costs 50 pizzas. After buying it, `helpers`{:class="block3variables"} is `1` and `helper price`{:class="block3variables"} is `58`.
