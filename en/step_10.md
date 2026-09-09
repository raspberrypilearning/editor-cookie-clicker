## Unlock the cutter

Make the cutter appear once the player can afford it.

<h2 class="c-project-heading--explainer">What you need to do</h2>

![The example project's cutter.](images/cutter.png)

## Step 1

Add the `Alert`{:class="block3sound"} sound to your equipment sprite.

Set up the cutter on the green flag: make it not draggable, switch to the plain costume, and hide it.

```blocks3
when green flag clicked
set drag mode [not draggable v]
switch costume to (cutter v)
hide
```

## Step 2

The cutter costs `25`, so wait until `pizzas`{:class="block3variables"} is greater than `24`. Then show it, play the alert, and tell the player what unlocked.

```blocks3
when green flag clicked
set drag mode [not draggable v]
switch costume to (cutter v)
hide
+wait until <(pizzas) > (24)>
+show
+start sound (Alert v)
+say [New equipment unlocked!] for (2) seconds
```

## Tip

An **unlock condition** is a rule that makes something available only after the player has done enough.

## Now run your code

Click until you reach 25 pizzas. The cutter appears.
