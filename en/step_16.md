## Make the chef variables

The chef is your first type of helper. Give it its own count and price variables.

<h2 class="c-project-heading--explainer">What you need to do</h2>

![The example project's robot chef.](images/chef.png)

## Step 1

Make a variable called `chefs`{:class="block3variables"} for how many chefs the player has hired.

Make another called `chef price`{:class="block3variables"} for how many pizzas the next chef costs.

## Step 2

Make a variable called `pizzas per second`{:class="block3variables"} for how many pizzas all the helpers make during each second.

Tick `chefs`{:class="block3variables"} and `pizzas per second`{:class="block3variables"} so the player can see them.

## Step 3

Click the `Stage`{:class="block3looks"} and give the variables starting values. The first helper costs `50`, so the cutter still unlocks first at `25`.

```blocks3
when green flag clicked
set [pizzas v] to (0)
set [pizzas per click v] to (1)
+set [chefs v] to (0)
+set [chef price v] to (50)
+set [pizzas per second v] to (0)
```

## Now run your code

Click the green flag. The new readouts show `chefs 0`, `chef price 50`, and `pizzas per second 0`.
