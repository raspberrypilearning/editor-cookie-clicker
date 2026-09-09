## Make the helper variables

The helper needs a few numbers to keep track of.

<h2 class="c-project-heading--explainer">What you need to do</h2>

![The example project's robot chef.](images/chef.png)

## Step 1

Make a variable called `helpers`{:class="block3variables"} for how many helpers the player has hired.

Make another called `helper price`{:class="block3variables"} for how many pizzas the next helper costs.

## Step 2

Make a variable called `pizzas per second`{:class="block3variables"} for how many pizzas all the helpers make during each second.

Tick `helpers`{:class="block3variables"} and `pizzas per second`{:class="block3variables"} so the player can see them.

## Step 3

Click the `Stage`{:class="block3looks"} and give the variables starting values. The first helper costs `50`, so the cutter still unlocks first at `25`.

```blocks3
when green flag clicked
set [pizzas v] to (0)
set [pizzas per click v] to (1)
+set [helpers v] to (0)
+set [helper price v] to (50)
+set [pizzas per second v] to (0)
```

## Now run your code

Click the green flag. The new readouts show `helpers 0`, `helper price 50`, and `pizzas per second 0`.
