## Add a small butterfly
Now, you will add a small butterfly that flies at a different angle and flies 'behind' the other butterflies.

--- task ---
Duplicate the **Butterfly 2** sprite to create a **Butterfly 3** sprite. 

--- /task ---

--- task ---

Change the colour of the **Butterfly 3** sprite so that it looks different to the others. 

--- /task ---

--- task ---
Make the **Butterfly 3** sprite fly in a different direction. What happens if you choose a negative number?

![Butterfly 3](images/butterfly-3-example.png)

**Tip:** Each sprite has its own costumes and code. Make sure that you select the correct sprite below the Stage before you click on their costumes or Code area. 

--- /task ---

--- task ---

Change the colour of the **Butterfly 3** sprite's wings. To do this, edit its costume with the **Fill** tool.

--- /task ---

All the butterflies are the same size. The scene will look more realistic if the **Butterfly 3** sprite is smaller and set behind the other butterflies.

--- task ---

Make the **Butterfly 3** sprite half the size (50%) of the other butterflies. Go to `Looks`{:class="block3looks"} and `set size to`{:class="block3looks"} to `50``%`{:class="block3looks"}:

```blocks3
when flag clicked
set rotation style [left right v]
point in direction (-45)
+set size to (50)%
forever
move (10) steps
if on edge bounce
end
```
--- /task ---

Now, you need to set the **Butterfly 3** sprite so that it is layered behind the other butterflies. 

--- task ---

Go to the `Looks`{:class="block3looks"} blocks menu again. Add a `go to front layer`{:class="block3looks"} block and select `back`{:class="block3looks"} in the drop-down menu:

```blocks3
when flag clicked
set rotation style [left right v]
point in direction (-45)
set size to (50)%
+go to [back v] layer
forever
move (10) steps
if on edge bounce
end
```
--- /task ---

--- task ---

Click on the green flag to check your program. Is the **Butterfly 3** sprite smaller than the other butterfly sprites? Also, is it flying behind them?

--- no-print ---

![Butterfly 3](images/butterfly-small-step4.gif)

--- /no-print ---

--- /task ---

--- save ---
