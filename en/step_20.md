## Start the clock

Set the helpers' numbers and add their pizzas every second.

![Selecting the Stage, to the right of the sprite list.](images/select-stage.png)

You're still working on the `Stage`{:class="block3looks"}.

Update the green flag script to set the new variables, work out the rate once, then add the pizzas-per-second every second.

```blocks3
when green flag clicked
set [pizzas v] to (0)
set [pizzas per click v] to (1)
+set [chefs v] to (0)
+set [chef price v] to (15)
+update pizzas per second
+forever
wait (1) seconds
change [pizzas v] by (pizzas per second)
end
```

## Now run your code

Buy a chef, then stop clicking.

Your `pizzas`{:class="block3variables"} keep rising on their own.
