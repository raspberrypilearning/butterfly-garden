## Add a butterfly
You're going to add a butterfly that flies left and right across the stage. 

+ Click 'Choose a Backdrop' and then select the 'Blue Sky' backdrop. 

![Choose the backdrop](images/butterfly-backdrop.png)

+ Delete the Cat sprite. 

![Choose the backdrop](images/butterfly-delete-cat.png)

+ Click 'Choose a Sprite' and add the 'Butterfly 1' sprite to your project.

![Choose the backdrop](images/butterfly-add-butterfly.png)

+ The butterfly is a bit big. Change its size to 50% (half as big).

![Choose the backdrop](images/butterfly-size-50.png)

+ Click on the Code tab and then 'Motion' to see the motion blocks. These blocks make sprites move around the stage. 

![Choose the backdrop](images/butterfly-motion)

+ Click on the `move (10) steps`{:class="block3motion"} block a few times and watch your butterfly move across the stage. 

Now you're going to make the butterfly move when your project is started by clicking the green flag above the stage. 

+ Drag a `when flag clicked`{:class="block3events"} block from `Events` to the stage. 

```blocks3
when flag clicked
```
The code under the `when flag clicked`{:class="block3events"} block will run when you click the green flag. 

+ Add a `forever`{:class="block3events"} block from `Control` and snap it in place under the `when flag clicked` block.

```blocks3
when flag clicked
+forever
end
```

Code blocks inside a `forever`{:class="block3control"} block will run over and over again. 

Tip: Notice the difference in colour between `Events` and `Control` blocks. 

+ Now add a `move (10) steps`{:class="block3motion"} block inside the `forever`{:class="block3events"} block.

```blocks3
when flag clicked
forever
+move (10) steps
end
```

+ Click the green flag to start your project. 

Your butterfly should fly to the right of the stage and then get stuck. 

![Butterfly right](images/butterfly-right.png)

+ To fix this, add an `if on edge bounce`{:class="block3motion"} block. This block makes a sprite flip its direction if it bumps into the edge of the screen. 

```blocks3
when flag clicked
forever
move (10) steps
+if on edge bounce
end
```

+ Click the green flag to restart your project and the butterfly should now fly across the stage, bouncing when it reaches the left and right edges. 
Did you spot a problem? The butterfly goes upside down when it flies to the left. This is because sprites point in the direction they are moving. 

![Butterfly right](images/butterfly-upside-down.png)

+ You can fix this by clicking on the `set rotation style [left-right]`{:class="block3motion"} block. 

![Butterfly left-right](images/butterfly-left-right.png)

+ Click the green flag again and your butterfly should stay the right way up!

The butterfly garden is supposed to be relaxing but the butterfly is flying very fast. 

+ Slow the butterfly down by changing the number of steps that it moves at a time from `10` to `2`:

```blocks3
when flag clicked
forever
+move (2) steps
if on edge bounce
end
```

+ Click the green flag and watch your butterfly move. 
















