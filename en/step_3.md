## Fly at an angle

Now, you will add another butterfly, but this time, it will fly at an angle to create a different flight pattern. 

The code for this butterfly will be similar to the code for the **Butterfly 1** sprite. You could add the code again, but it is quicker to duplicate (copy) the sprite. 

--- task ---
Right-click on the **Butterfly 1** sprite in the Sprite list below the Stage (or if you are using a tablet, tap and hold) and select **duplicate** in the menu that appears:

![Open the right-click menu for Butterfly 1](images/butterfly-duplicate.png){:width="400px"}

--- /task ---

This will create a copy of the **Butterfly 1** sprite called **Butterfly 2**. 

![Butterfly 2 sprite](images/butterfly-butterfly-2.png){:width="400px"}

The costumes, code, and settings, such as the size and rotation style, are copied to the new sprite. 

--- task ---
Click on the green flag to see both butterflies move. 

--- /task ---

--- task ---
Click on the red stop button above the Stage to stop the butterflies moving. 

![Butterfly 2 sprite](images/butterfly-stop.png){:width="400px"}

--- /task ---

Now, you will change the colour of the **Butterfly 2** sprite so that you can tell them apart easily. 

--- task ---
Click on the **Butterfly 2** sprite in the Sprite list below the Stage.

![Select butterfly 2](images/butterfly-2-under-stage.png)
--- /task ---

--- task ---
Click on the **Costumes** tab. 

![Butterfly 2 Costumes tab](images/butterfly-costumes-2.png){:width="300px"}

--- /task ---

--- task ---
Click on the **Fill** (paint bucket) tool.  

![Butterfly 2 Costumes tab](images/butterfly-fill-tool.png)

--- /task ---

--- task ---
Click on the **Fill** colour and change the sliders to get a colour that you like. 

![Butterfly 2 Costumes tab](images/butterfly-fill-colour.png)

--- /task ---

--- task ---
Click on the green parts of the butterfly's wing to fill them with your new colour. 

![Butterfly 2 Costumes tab](images/butterfly-fill-wings.png)

--- /task ---

The colour of the **Butterfly 2** sprite will also change on the Stage and in the Sprite list below the Stage. 

![Butterfly 2 Costumes tab](images/butterfly-colour-changed.png)

--- task ---
The **Butterfly 2** sprite also has its own code. Make sure that the **Butterfly 2** sprite is still selected in the Sprite list below the Stage and click on the **Code** tab. 

--- /task ---

The **Butterfly 2** sprite has the same code as the **Butterfly 1** sprite. You will change it so that the **Butterfly 2** sprite flies in a different pattern.

--- task ---
Add a `point in direction`{:class="block3motion"} block after the `set rotation style [left-right]`{:class="block3motion"} block. A gap will open up and the block will fit into place:

```blocks3
when flag clicked
set rotation style [left-right v]
+point in direction (90)
forever
move (2) steps
if on edge, bounce
end
```

--- /task ---

The number `90` in the `point in direction`{:class="block3motion"} block means 'point to the right', which is why the butterfly flies to the right at first. `0` means 'point up towards the top of the Stage'. You will make the **Butterfly 2** sprite fly at a 45-degree angle. 

--- task ---
Click on the number `90` in the `point in direction`{:class="block3motion"} block and change the number to `45`. To do this, you can move the arrow that appears, or type `45`.

![Selecting 45 degree angle](images/butterfly-set-angle.png)

--- /task ---

--- task ---
Check that your code looks like this:

```blocks3
when flag clicked
set rotation style [left-right v]
+point in direction (45)
forever
move (2) steps
if on edge, bounce
end
```
--- /task ---

--- task ---
Click on the green flag to see the **Butterfly 2** sprite move in its new pattern.

--- /task ---

--- save ---
