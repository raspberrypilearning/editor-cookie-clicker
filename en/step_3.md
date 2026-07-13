## Add a click sound

A click feels better with a sound.

![the pizza sprite](images/pizza.png)

Open the **Sounds** tab, click the speaker icon, and pick something short.

![The Sounds tab at the top-left of the editor.](images/sounds_tab.png)

Add it to the top of your script.

Use `start sound`{:class="block3sound"} in this project, not `play sound until done`{:class="block3sound"}, so the sound starts without holding up the rest of the program.

```blocks3
when this sprite clicked
+start sound (Tennis Hit v)
change [pizzas v] by (1)
```

## Tip

Code that starts something and then keeps going is called **non-blocking**, because it does not pause the rest of the program.

## Now run your code

Click your sprite.

You hear the sound the moment you click.
