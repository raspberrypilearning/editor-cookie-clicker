## Make the pizza bounce

Give the pizza a bit of life when it's clicked.

![the pizza sprite](images/pizza.png)

Make the sprite bounce a little each time.

```blocks3
when this sprite clicked
start sound (Tennis Hit v)
change [pizzas v] by (1)
+change size by (10)
+wait (0.05) seconds
+change size by (-10)
```

## Now run your code

Click your sprite.

It pops bigger for a moment with every click.
