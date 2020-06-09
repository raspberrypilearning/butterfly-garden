## Add a small butterfly

Duplicate Butterfly 2 to create Butterfly 3. Use what you have learned to make this butterfly different to the others. 

--- task ---
Change the colour of the butterfly's wings by editting its costume with the Fill tool.

Make your butterfly fly in a different direction. What happens if you choose a negative number?

![Butterfly 3](images/butterfly-3-example.png)

__Tip:__ Make sure you select the sprite you want to change under the stage before clicking on 'Costumes' or 'Code'. Each sprite has its own costumes and code. 

--- /task ---

All the butterflies are the same size. The scene will look more realistic if Butterfly 3 is smaller and set behind the other butterflies.

Make Butterfly 3 half the size (50%) of the other butterflies. Go to `Looks`{:class="block3looks"} and set size to (50)% {:class="block3looks"}

```blocks3
when flag clicked
set rotation style [left right v]
point in direction (90)
+set size to (50)%
forever
move (10) steps
if on edge bounce
end
```
--- task ---

--- /task ---

All the butterflies are the same size. The scene will look more realistic if Butterfly 3 is smaller and set behind the other butterflies.

Make Butterfly 3 half the size (50%) of the other butterflies. Go to `Looks`{:class="block3looks"} and set size to (50)% {:class="block3looks"}

```blocks3
when flag clicked
set rotation style [left right v]
point in direction (90)
+set size to (50)%
forever
move (10) steps
if on edge bounce
end
```
--- task ---

