## Start the clock

Recount the earning rate after every purchase, then add that many pizzas every second.

## Step 1

Return to the helper sprite. Broadcast `update`{:class="block3events"} at the end of its buy script.

```blocks3
when this sprite clicked
if <(pizzas) > ((helper price) - (1))> then
start sound (Clang v)
change [pizzas v] by ((0) - (helper price))
change [helpers v] by (1)
set [helper price v] to (round ((helper price) * (1.15)))
+broadcast (update v)
end
```

## Step 2

On the `Stage`{:class="block3looks"}, replace the fixed `pizzas per second`{:class="block3variables"} setup with your custom block. Then add the game's clock.

```blocks3
when green flag clicked
set [pizzas v] to (0)
set [pizzas per click v] to (1)
set [helpers v] to (0)
set [helper price v] to (50)
+update pizzas per second :: custom
+forever
wait (1) seconds
change [pizzas v] by (pizzas per second)
end
```

## Tip

A regular moment when a game updates its numbers is called a **tick**. This clicker has one tick every second.

## Now run your code

Earn 50 pizzas and buy one helper. Check that `pizzas per second`{:class="block3variables"} becomes `1`, then stop clicking. The score rises by one every second.

The helper is a repeatable upgrade. When the score reaches its new price, the same sprite appears again so the player can hire another one.
