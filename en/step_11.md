## Buy the cutter

Let the player click the cutter to upgrade their clicks.

![The pizza shop's cutter.](images/cutter.png)

You're still working on the `Cutter`{:class="block3looks"} sprite.

Clicking it upgrades the player's clicks, switches to the "bought" costume, and shuts itself off so it can't be bought twice.

```blocks3
when this sprite clicked
start sound (Tada v)
set [pizzas per click v] to (2)
next costume
stop [other scripts in sprite v]
stop [this script v]
```

## Now run your code

Reach 25 pizzas, then click the cutter.

Every click is now worth 2 pizzas.
