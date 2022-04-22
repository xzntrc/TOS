# Programs
Now that we've understood the UI, let's explore some programs on TempleOS. From the start, we have two terminal sessions open and AutoComplete running on the screen. Let's close all three of these, start off by hiding AutoComplete with <kbd>Shift+Alt+A</kbd>, next close the two open terminals by pressing the close button in the right corner or by pressing our abort keybinding (<kbd>Shift+Esc</kbd>). Upon closing the running programs, we are exposed to our wallpaper. On the bottom is an immovable task list, above it is a program called "Adam".

### Adam
"This is the adam task, he's- it's like Adam and Eve; he's the first task created at startup." - [Terry A. Davis](https://youtu.be/jCkZmIoZS1c?t=187). At startup, the Adam task is created and appears in the little window at the top beneath the user terminal windows. Because the Adam task is immutable, any memory objects that you don't want destroyed by the death of any one job are stored on Adam's heap. Adam executes the file `::/StartOS.HC` (`:` refers to the boot drive), when the Adam task is created. 

### Personal Menu
Press <kbd>Ctrl+M</kbd> within a terminal to get to your Personal Menu, if you aren't in a terminal, press <kbd>Ctrl+Alt+T</kbd>. Your Personal Menu is exactly that; a customizable menu that houses links to programs, games, and files. You can click on items within your Personal Menu using your mouse. The Personal Menu is a standard [DolDoc](./doldoc.md) document; The DolDoc filetype is one of the most intriguing and underappreciated features of TempleOS, allowing you to embed 3D models and photos in documents and show them on the terminal. The Personal Menu is stored in `C:/Home/PersonalMenu.DD.Z`, we will be exploring how to edit files in a future chapter (it's also worth mentioning that `.Z` means that a file is compressed), for now, just know that the Personal Menu is your portal to all cool things in TempleOS; have fun and explore everything in it.

#### Fun Games
Games in TempleOS are categorized as being "Fun" and "Unfun".
<details>
<summary><b>Titanium</b></summary>
<br>
In Titanium, you play as a Jet/Plane from a top-down perspective over land. Collect points as you shoot at enemies. You move with your arrow keys and shoot with <kbd>Space</kbd>. Titanium is one of my favorite games in TempleOS; it reminds me of Galaga except it's on Earth and the enemies don't fire back.
</details>
<br>
<details>
<summary><b>Black Diamond</b></summary>
<br>
In Black Diamond, you play as a person skiing down a mountain, with the objective to not hit into trees, rocks, and what I presume are mountain lions, you are penalized for hitting into these objects. Your goal is to obtain a small enough penalty.
<br>
</details>
<br>
<details>
<summary><b>Flap Bat</b></summary>
<br>
In Flap Bat, you play as a bat whose goal is to eat bugs. The bugs are a fixed amount that cycle through, your goal is to eat all of them in the lowest time possible. Press <kbd>Space</kbd> to flap and hold to glide; spamming does nothing but make you fall, the best way is to flap at a consistent speed.
<br>
</details>
<br>
<details>
<summary><b>Varoom</b></summary>
<br>
In Varoom you play as a car, with the objective to complete the whole track in the shortest time possible, on the course are computer generated players; running into them causes a "Game Over". Control the car using your arrow keys.
<br>
</details>
<br>
<details>
<summary><b>FlatTops</b></summary>
<br>
Flattops is a warship game against a computer player. Your goal is to destroy the other ships while launching squadrons. Left Mouse to change course of the squadrons, and Right Mouse to deploy squadrons.
<br>
</details>
<br>
<details>
<summary><b>Bomber Golf</b></summary>
<br>
In Bomber Golf you play as a bomber plane, your objective is to destroy the enemy in the fewest amount of moves, hence "Golf". Move using your arrow keys and release a bomb with <kbd>Space</kbd>.
<br>
</details>
<br>
<details>
<summary><b>Keep Away</b></summary>
<br>
Keep Away is a basketball-like game in which there are 2 teams, your goal is to pass the ball between your team and intercept the ball from the opponent. Your character follows your mouse, Left Click to pass the ball, and Right Click to jump.
<br>
</details>
<br>
<details>
<summary><b>Raw Hide</b></summary>
<br>
In RawHide your objective is to herd cattle into a coral located in the top left. Your character follows your mouse, hold <kbd>Ctrl+LMB</kbd> to scroll up.
<br>
</details>



