## Add more equipment

Two more pieces let the player keep upgrading.

![The pizza shop's rolling pin.](images/rolling_pin.png)

Copy the two cutter scripts by dragging each onto the new sprite in the sprite list, then change the numbers.

--- no-print ---

![Dragging a script onto another sprite in the sprite list to copy it.](images/drag-script-to-sprite.gif)

--- /no-print ---

## Step 1

Add the rolling pin.

It appears above `499` pizzas and sets `pizzas per click`{:class="block3variables"} to `6`.

Save [the rolling pin sprite](images/rolling_pin.png) and import it with **Upload** if you want to use the pizza shop's equipment.

```blocks3
when green flag clicked
set drag mode [not draggable v]
switch costume to (rolling_pin v)
forever
if <(pizzas) > (499)> then
start sound (Alert v)
show
else
hide
end
end
```

```blocks3
when this sprite clicked
start sound (Tada v)
set [pizzas per click v] to (6)
next costume
stop [other scripts in sprite v]
stop [this script v]
```

## Step 2

Add the oven the same way.

It appears above `3000` pizzas and sets `pizzas per click`{:class="block3variables"} to `24`.

Give each sprite its own first costume in its "appear" script.

Save [the oven sprite](images/oven.png) and import it with **Upload** if you want to use the pizza shop's equipment.

![The pizza shop's oven.](images/oven.png)

## Now run your code

Play until you can buy the rolling pin and the oven.

Each one makes your clicks worth even more.
