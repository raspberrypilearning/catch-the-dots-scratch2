## High score

You're going to save the game's high score, so that players can see how well they are doing.

--- task ---
Create a new variable called `high score`{:class="blockdata"}.

![Stage sprite](images/stage-sprite.png)

--- /task ---

--- task ---
Select the Stage, and create a new custom block called `check high score`{:class="blockmoreblocks"}.

![Stage sprite](images/stage-sprite.png)
![screenshot](images/dots-custom-1.png)

--- /task ---

--- task ---
Add code to your custom block so that the block checks if the current value of `score`{:class="blockdata"} in larger than the value of the `high score`{:class="blockdata"} variable, and then stores the value of `score`{:class="blockdata"} as the new value of `high score`{:class="blockdata"}.

![Stage sprite](images/stage-sprite.png)

```blocks
	define [check high score]
	if <(score) > (high score)> then
		set [high score v] to (score)
	end
```
--- /task ---

--- task ---
Add your new custom block to the Stage script before the end of the script.

![Stage sprite](images/stage-sprite.png)
```blocks
when flag clicked
set [lives v] to (3)
set [score v] to (0)
wait until <(lives) < (1)>
+ check high score
stop [all v]
```

--- /task ---

--- task ---

Play your game twice to check whether your score gets correctly saved as the `high score`{:class="blockdata"}.

--- /task ---
