## Show the chef when affordable

Make the chef appear only when the player can pay for it.

![The pizza shop's robot chef.](images/chef.png)

You're still working on the `Chef`{:class="block3looks"} sprite.

This script also tells the game to recount the pizzas-per-second whenever things change.

```blocks3
when green flag clicked
set drag mode [not draggable v]
forever
if <(pizzas) > ((chef price) - (1))> then
show
else
hide
end
broadcast (update v)
end
```

The `broadcast (update v)`{:class="block3events"} won't do anything yet.

You'll build what listens for it on the Stage next.
