## Predict the winner

### Video of this step

<video width="960" height="540" controls>
  <source src="images/part2.mp4" type="video/mp4" alt="A video walkthrough of this step">
Your browser does not support the video tag.
</video>

### Add a button block

--- task ---

- From the `Input`{:class="microbitinput"} menu, drag the `on button [A] pressed`{:class="microbitinput"} block to the code editor panel.

--- /task ---

--- task ---

- From the `Basic`{:class="microbitbasic"} menu, drag the `clear screen`{:class="microbitbasic"} block into the code editor.
- Place it inside the `on button [A] pressed`{:class="microbitinput"} block.
 
--- /task ---

--- task ---

- From the `Basic`{:class="microbitbasic"} menu, drag the `show string`{:class="microbitbasic"} block into the code editor.

- Place it inside the `on button [A] pressed`{:class="microbitinput"} block, under the `clear screen`{:class="microbitbasic"} block.
  
```microbit
input.onButtonPressed(Button.A, function () {
    basic.clearScreen()
    basic.showString("Hello!")
})
```

--- /task ---

### Use randomness!

--- task ---

- From the `Arrays`{:class="microbitarrays"} menu, drag the `get random value from [list]`{:class="microbitarrays"} block into the code editor. 

- Change `list`{:class="microbitvariables"} to `text list`{:class="microbitvariables"}.

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

### Test in the emulator

--- task ---

- Wait for the stick figure to show and then press button A.

- Check one of your teams/players displays.

--- /task ---

### Download

--- task ---

Download your program onto your micro:bit!

--- /task ---

[[[download-to-microbit]]]

### Test on your micro:bit

--- task ---

- Wait for the stick figure to show and then press button A.

You have your winner!

--- /task ---
