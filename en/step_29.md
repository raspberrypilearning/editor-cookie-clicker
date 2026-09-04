## Animate the helpers

Give the helpers a gentle pulse so they look busy at work.

![The example project's robot chef.](images/chef.png)

## Step 1

Add this script to your first helper. It grows the sprite a little, then shrinks it back.

```blocks3
when green flag clicked
forever
repeat (5)
change size by (2)
wait (0.05) seconds
end
repeat (5)
change size by (-2)
wait (0.05) seconds
end
end
```

## Step 2

Drag the script onto your other helper to copy it.

## Tip

Small animations that make a game feel lively without changing its rules are part of **game feel**, sometimes called **juice**.

## Now run your code

Click the green flag. Each helper grows by 10 in total, shrinks by 10, and returns to its starting size before the next pulse.

Leave the game running and check that the helpers keep pulsing while the score still rises every second. Remember to save your project.
