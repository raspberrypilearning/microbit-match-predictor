## Predict the winner

Use randomness to predict an outcome!

--- task ---

- From the `Input`{:class="microbitinput"} menu, drag the `on button [A]`{:class="microbitinput"} block to the code editor panel.

--- /task ---

--- task ---

- From the `Basic`{:class="microbitbasic"} menu, drag the `clear screen`{:class="microbitbasic"} block into the code editor.
- Place it inside the `on button [A]`{:class="microbitinput"} block.
 
--- /task ---

--- task ---

- From the `Basic`{:class="microbitbasic"} menu, drag the `show string`{:class="microbitbasic"} block into the code editor.

- Place it inside the `on button [A]`{:class="microbitinput"} block, under the `clear screen`{:class="microbitbasic"} block
  
```microbit
input.onButtonPressed(Button.A, function () {
    basic.clearScreen()
    basic.showString("Hello!")
})
```

--- /task ---

--- task ---

- Click `Advanced`. 

- From the `Arrays`{:class="microbitarrays"} menu, drag the `get random value from [list]`{:class="microbitarrays"} block into the code editor. 
Change `list`{:class="microbitvariables"} to `text list`{:class="microbitvariables"}.

```microbit
input.onButtonPressed(Button.A, function () {
    basic.clearScreen()
    basic.showString("" + (text_list._pickRandom()))
})
let text_list: string[] = []
basic.showIcon(IconNames.StickFigure)
text_list = ["Team A", "Team B"]

```
--- /task ---

--- task ---

Download your program onto your micro:bit!

--- /task ---

[[[download-to-microbit]]]

### Test your program

--- task ---

Wait for the stick figure to show and then press button A.

You have your winner!

--- /task ---

Here are some more examples of people having fun with this project!

<html>
<video width="480" height="640" controls>
<source src="images/predict1.mp4" type="video/mp4" alt="Someone using their micro:bit to predict the winner of a football tournament">
Your browser does not support the video tag.
</video>

<video width="480" height="640" controls>
<source src="images/predict2.mp4" type="video/mp4" alt="Someone using their micro:bit to predict the winner of a tennis tournament">
Your browser does not support the video tag.
</video>
</html>
