## Show the cutter when affordable

Make the cutter appear only once the player can pay for it.

![The pizza shop's cutter.](images/cutter.png)

You're still working on the `Cutter`{:class="block3looks"} sprite.

```blocks3
when green flag clicked
set drag mode [not draggable v]
switch costume to (cutter v)
forever
if <(pizzas) > (25)> then
start sound (Alert v)
show
else
hide
end
end
```

## Tip

An **unlock condition** is a rule that makes something available only after the player has done enough.

## Now run your code

Click until you pass 25 pizzas.

The cutter appears.
