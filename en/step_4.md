## More dots

--- task ---
Duplicate your 'red' dot sprite twice, and name the two new sprites 'yellow' and 'blue'.

![screenshot](images/dots-more-dots.png)
--- /task ---

--- task ---
Change the costume of each new sprite so it is the correct colour: the 'yellow' sprite should be yellow, and the 'blue' sprite should be blue.
--- /task ---

--- task ---
Change the code of each sprite so that the player has to match dot clone to the correct colour on the controller to score points.

![screenshot](images/dots-all-test.png)

--- hints ---
--- hint ---
This is the code you need to find and alter for both new sprites:

![screenshot](images/dots-more-dots.png)

```blocks
	if <touching color [#FF0000]?> then
		change [score v] by (1)
		play sound [pop v]
        ...
	end
```
--- /hint ---
--- hint ---
This is how you need to change the code for the yellow sprite:
```blocks
	if <+ touching color [#FFFF00]?> then
        change [score v] by (1)
        play sound [pop v]
	end
```

This is how you need to change the code for the blue sprite:
```blocks
	if <+ touching color [#0000FF]?> then
        change [score v] by (1)
        play sound [pop v]
	end
```
--- /hint ---
--- /hints ---
--- /task ---

If you play the game now, you can see that the dots sometimes get created one top of each other.

--- task ---
Add code to the 'yellow' dot sprite so that it waits 4 seconds after the flag is clicked before appearing.

![screenshot](images/dots-more-dots.png)

```blocks
	when flag clicked
	hide
	+ wait (4) secs
```

Then add code to the 'blue' dot sprite so that it waits 6 seconds after the flag is clicked before appearing.

--- /task ---
