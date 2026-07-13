## Wire up the granny

Point the copied scripts at the granny's own numbers.

![The pizza shop's granny.](images/granny.png)

## Step 1

In the copied buy script, swap the chef variables for the granny ones and pick a different sound.

```blocks3
when this sprite clicked
start sound (Collect v)
change [pizzas v] by ((0) - (granny price))
change [grannies v] by (1)
set [granny price v] to (round ((granny price) * (1.15)))
```

## Step 2

Swap the variables in the copied appear script too.

```blocks3
when green flag clicked
set drag mode [not draggable v]
forever
if <(pizzas) > ((granny price) - (1))> then
show
else
hide
end
broadcast (update v)
end
```

The granny won't add anything yet.

You'll make her count towards your pizzas-per-second next.
