## Add your teams/players

Choose two or more teams or players that have a big game soon.

### Open MakeCode

--- task ---

Open the MakeCode editor at [makecode.microbit.org](https://makecode.microbit.org){:target="_blank"}.

--- /task ---

--- collapse ---

---
title: Offline version of the editor
---

There is also a [downloadable version of the MakeCode editor](https://makecode.microbit.org/offline-app){:target="_blank"}.

--- /collapse ---

### Create a new project

--- task ---

Click on the **New Project** button.

<img src="images/new-project-button.png" alt="The New Project button inside MakeCode." width="250"/>

--- /task ---

### Name your project

--- task ---

Give your new project the name `match predictor` and click **Create**.

--- /task --- 

### Show an icon

--- task ---

- From the `Basic`{:class="microbitbasic"} menu, drag the `show icon`{:class="microbitbasic"} block into the code editor. 
  
- Place it inside the  `on start`{:class="microbitbasic"} block. 

- Select the stick figure icon to show when the micro:bit is ready.

```microbit
basic.showIcon(IconNames.StickFigure)
```
--- /task ---

### Add your teams/players

--- task ---
  
- Click `Advanced`. 

- From the `Arrays`{:class="microbitarrays"} menu, drag the `set [text list]`{:class="microbitvariables"} block into the code editor. 

- Place it in the `on start`{:class="microbitbasic"} block under the icon.

```microbit
basic.showIcon(IconNames.StickFigure)
let text_list = ["a", "b", "c"]
```

--- /task ---

--- task ---

Replace the items `a`, `b`, `c` with the names of your teams/players. 
(We have used `Team A` and `Team B` in the example - we're not taking sides!)

**Tip**: If you only need two, you can delete the last one in the array by pressing the `-` symbol. 

If need more, you can add one to the end of the array by pressing the `+` symbol. 

```microbit
basic.showIcon(IconNames.StickFigure)
let text_list = ["Team A", "Team B"]
```

--- /task ---
