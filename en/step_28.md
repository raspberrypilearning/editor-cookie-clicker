## Animate the equipment

Make the equipment wiggle so the shop feels alive.

<h2 class="c-project-heading--explainer">What you need to do</h2>

![The example project's cutter.](images/cutter.png)

## Step 1

Add this script to your first piece of equipment. The `point in direction`{:class="block3motion"} block starts it level each time you click the green flag, then it rocks back and forth forever.

```blocks3
when green flag clicked
point in direction (90)
forever
turn right (10) degrees
wait (0.2) seconds
turn left (10) degrees
wait (0.2) seconds
turn left (10) degrees
wait (0.2) seconds
turn right (10) degrees
wait (0.2) seconds
end
```

## Step 2

Drag the script onto your other equipment sprites to copy it to each one.

## Now run your code

Click the green flag. Each equipment sprite rocks gently and returns to its starting direction after every wiggle.
