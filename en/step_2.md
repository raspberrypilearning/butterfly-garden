## Add a butterfly
You're going to add a butterfly that flies left and right across the stage. 

--- task ---

Open a new Scratch project.

**Online:** open a new online Scratch project at [rpf.io/scratch-new](http://rpf.io/scratch-new){:target="_blank"}.

**Offline:** open a new project in the offline editor.

If you need to download and install the Scratch offline editor, you can find it at [rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}.

--- /task ---

--- no-print ---

Watch this short video which shows what to do next.

![screenshot](images/butterfly-setup-step2.gif) 

--- /no-print ---

Follow each task given below.

--- task ---
Click **Choose a Backdrop** and then select the **Blue Sky** backdrop. 

![Choose the backdrop](images/butterfly-backdrop.png)
--- /task ---

--- task ---
Delete the Cat sprite. 

![Delete the cat](images/butterfly-delete-cat.png)

--- /task ---

--- task ---
Click **Choose a Sprite** and add the **Butterfly 1** sprite to your project.

![Add the butterfly 1 sprite](images/butterfly-add-butterfly.png)

--- /task ---

--- task ---
Now title and save your project so far. Go to **File** in the menu. If you have a Scratch account, click **Save now**. If you don't have an account click **Save to your computer**.

![Save  project](images/butterfly-save.png)
--- /task ---

--- no-print ---

Watch this short video which shows what to do next.

![screenshot](images/butterfly-move-step2.gif)

--- /no-print ---

Follow each task given below.

--- task ---
Click on the code tab and then select `Motion`{:class="block3motion"} to see the motion blocks available. These blocks make sprites move around the stage. 

![Open the Motion section](images/butterfly-motion.png){:width="300px"}
--- /task ---

--- task ---
Click on the `move (10) steps`{:class="block3motion"} block a few times and watch your butterfly move across the stage. 
--- /task ---

Now you're going to make the butterfly move when your project is started by clicking the green flag above the stage. 

![Green flag above the stage](images/butterfly-green-flag.png){:width="400px"}

--- task ---
From `Events`{:class="block3events"}, select a `when flag clicked`{:class="block3events"} block and drag it in to the code area. 

```blocks3
when flag clicked
```
The code under the `when flag clicked`{:class="block3events"} block will run when you click the green flag. 

--- /task ---

--- task ---
From `Control`{:class="block3control"}, add a `forever`{:class="block3control"} block and snap it in place under the `when flag clicked`{:class="block3events"} block.

```blocks3
when flag clicked
+forever
end
```

Code blocks inside a `forever`{:class="block3control"} block will run over and over again. 

**Tip:** Notice the subtle colour difference between `Events`{:class="block3events"} (yellow) and `Control`{:class="block3control"} (orange) blocks.

--- /task ---

--- task ---
Now add a `move`{:class="block3motion"} `10` `steps`{:class="block3motion"} block inside the `forever`{:class="block3events"} block.

```blocks3
when flag clicked
forever
+move (10) steps
end
```

--- /task ---

--- task ---
Click the green flag to start your project. 

Your butterfly should fly to the right of the Stage and then get stuck.

![Butterfly at right of stage](images/butterfly-right.png){:width="400px"}

--- no-print ---

Watch this short video. Is your butterfly getting stuck like this?

![screenshot](images/butterfly-stuck-step2.gif)

--- /no-print ---

--- /task ---

--- task ---
To fix the stuck butterfly, add an `if on edge bounce`{:class="block3motion"} block. This block makes a sprite flip its direction if it bumps into the edge of the screen. 

```blocks3
when flag clicked
forever
move (10) steps
+if on edge bounce
end
```
--- /task ---

--- task ---
Click the green flag to restart your project and the butterfly should now fly across the stage, bouncing when it reaches the left and right edges. 
--- /task ---

Did you spot an issue? The butterfly goes upside down when it flies to the left. This is because sprites point in the direction they are moving. 

![Butterfly upside down when flying left](images/butterfly-upside-down.png){:width="400px"}

--- task ---
You can fix this by adding a `set rotation style [left-right]`{:class="block3motion"} block under `when flag clicked`{:class="block3events"}.

![Set butterfly left-right rotation style](images/butterfly-left-right.png){:width="400px"}

```blocks3
when flag clicked
+set rotation style [left right v]
forever
move (2) steps
if on edge bounce
end
```

--- /task ---

--- task ---
Click the green flag again and your butterfly should stay the right way up!
--- /task ---

The butterfly garden is supposed to be relaxing but the butterfly is flying very fast. 

--- task ---
Slow the butterfly down by changing the number of steps that it moves at a time from `10` to `2`:

```blocks3
when flag clicked
forever
set rotation style [left right v]
+move (2) steps
if on edge bounce
end
```
--- /task ---

--- task ---
Click the green flag and watch your butterfly move. 
--- /task ---

--- save ---













