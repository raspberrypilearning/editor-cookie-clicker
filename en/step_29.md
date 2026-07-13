## Animate the auto-clickers

Give your helpers a gentle pulse so they look busy at work.

![The pizza shop's robot chef.](images/chef.png)

## Step 1

Add this script to your first helper.

It grows the sprite a little, then shrinks it back, over and over.

```blocks3
when green flag clicked
forever
repeat (5)
  change size by (2)
  wait (0.05) seconds
end
repeat (5) times
wait (0.05) seconds
change size by (-2)
end
end
```

## Step 2

Add the same script to your other helper by dragging it onto them in the sprite list.

## Now run your code

Click the green flag.

Your helpers pulse away while they make pizzas.

Your pizza shop is complete.
