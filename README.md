### What Is ASOIAF-Simulator?

ASOIAF-Simulator is a no-cost, web-based, fan-created simulator that leverages Phaser JS to emulate the [A Song of Ice and Fire](https://cmon.com/product/a-song-of-ice-fire-tmg) tabletop miniature game (made by [CMON](https://asoiaf.cmon.com/)), in a vivid 2D environment.

To play, visit:

[asoiaf-sim.com](http://asoiaf-sim.com/)

### How To Demo Video:

[![Embedded YouTube Video](https://img.youtube.com/vi/0q5gF5QeRR8/0.jpg)](https://www.youtube.com/watch?v=0q5gF5QeRR8)

### Features:

* 2-player ASOIAF simulation
* Unit Creation/Movement - create ASOIAF Units/Attachments/NCUs with movement controls
* Unit movement history - Press the `r` button to have a unit revert to it's last position.
* Units have short-range, long-range and line of sight arcs built-in.
* Tactics board - with turn token and player turn throne token.
* Battlemaps - Currently we have 8 battlemaps that you can select from. (battlemaps are not synced between players so you can set to whatever you want on your side)
* Objective Cards - objective cards deck built-in
* Mission Cards - Mission cards deck built-in
* Tactics Cards/Deck selection.
* Dice - Builtin dice system for a max of 20x D6 dice. The first dice (in gold border) can be used to represent a D3.
* Dice - Dice history
* Tape-Measures - automatic tape measures on units. You can also trigger a manual tape measure by holding down `T` key.
* Cards - All Units/Tactics/NCU/Attachment/etc... cards built-in.
* EN, FR, DE translations for data cards.
* Color Selection - Army color selection so you can customize your units trays/colors.
* Save Game State - Save the simulators current game state and copies it to the clipboard.
* Import Data/Saves from a [asoiaf-stats.com](https://asoiaf-stats.com/) list TTS export, CMONs list export from [War Council](https://play.google.com/store/apps/details?id=com.cmon.asif&hl=en_US&gl=US), and ASOIAF-Simulator game state saves. 
* Simulator Log - Important actions are logged and can be viewed under the HELP menu. (this is helpful to keep people honest).
* Set Names - players can set their name by selecting P1: or P2: (depending if you joined as player 1 or player 2)
* Tactics/Mission/Objectives cards and Dice rolls all use the JavaScript `crypto` server-side to ensure things cryptographically secure/random.

### Requirements:

* **For Best Results** - Use a 1920x1080 (16:9 aspect ratio) screen and full-screen (F11)
* Web Browser (preferably **Chrome** since thats the only browser I tested in.)
* Mouse and Keyboard
* Internet

### Key Bindings:

* When you have a moveable object selected you can use `WASD` to move it.
* Also when selected, you can rotate an object using `Q` to rotate counter-clockwise and `E` to rotate clockwise.
* When moving/rotating objects, you can hold down `SHIFT` to speed-up the `WASD` or `Q` / `E` rotation.
* Tape-Measure - Using your mouse, move to the position you want then hold down `T` and drag the mouse. This will allow you to measure what would be in inches.
* Delete - Select and object and press `Del` to delete
* Reset Object Position - Select and then deselect a unit and press `R` to reset it to its last position

### Known Issues:

* Cards aren't perfect. Im working on them at https://github.com/chrisjd20/asoiaf_card_generator
* Translations only apply to EN,FR,DE and only apply to most card images when not specifying english. Otherwise most of the site is only in english.
* The import feature from TTS needs work. This is because their IDS frot the cmond cards uses historical data from years. Mine is only the most recent. Will have to find some way to fix this.

### Filing Issues:

Please feel free to file any issues you may experiencing here in this github repo. For bugs or issues, it will help if you include screenshots and perhaps any javascript errors that you may experience. On Chrome you can open the developer tools to the javascript console by:

1. **Open Google Chrome**: Start by opening your Google Chrome browser.

2. **Navigate to the Desired Page**: Go to the web page where you want to inspect or debug using the developer tools.

3. **Open Developer Tools**: You can open the Chrome Developer Tools in several ways:
    - Press `Ctrl` + `Shift` + `I` (Windows/Linux) or `Cmd` + `Option` + `I` (Mac).
    - Right-click on any page element and select `Inspect`.
    - Go to the Chrome menu at the top-right (three dots), then select `More Tools` > `Developer Tools`.

4. **Access the JavaScript Console**: 
    - Once the Developer Tools pane is open, click on the `Console` tab to switch to the JavaScript console.
    - Alternatively, you can press `Ctrl` + `Shift` + `J` (Windows/Linux) or `Cmd` + `Option` + `J` (Mac) to open Developer Tools directly to the Console tab.

5. **Ready to Use**: Now you can view console logs, and report any errors that might be displayed there.


### TODO LIST:

- [x] Basic Layout with battle maps and tactics board
- [x] Buttons to include Army color Selector
- [x] Player Name Change
- [x] Card Generator
- [x] Units
- [x] NCU's
- [x] Attachments
- [x] Game Objects
- [x] Server-side setup
- [x] Networking for all non-ui in-game objects
- [x] Support EN / FR / DE
- [x] Import Army Lists from Stats / War Council
- [x] Dice System (uses crypto module server-side for cryptographically secure/random dice rolling)
- [x] Tactics Cards (uses crypto module server-side for cryptographically secure/random card shuffling)
- [x] Missions Cards
- [x] Tactics Selection Filters Out (Mostly) Invalid Commander Choices
- [x] Objectives Cards
- [x] Actions Log Stored Server Side (dice rolls, tactics/missions card actions, Army movements/attribute changes) ( this is viewable in help/?)
- [x] Important actions logged to toasts
- [x] Game State Save System and Save Reload
- [x] Mouse/Hand for UI component
- [x] D3 into dice system ( Just use the one dice in a gold border as the D3 )
- [x] Need to have finished moves/certain attr changes added to log for tray objects
- [x] mouse out of background causes stop drag? - fixed this by tracking all mouse up to trigger stop dragging
- [x] Toggle Turn and player order throne Turn Token
- [x] straight arrows coming off trays to show movement
- [x] Toggle All Units Ranges/Graphics
- [x] Create landing page
- [x] Help/How To finished (with how to video perhaps?)
- [ ] Add additional terrain
- [ ] Better logic for initally placement of units/ncus/attachements (and their cards) during creation
- [ ] Object Position History will be serverside instead of only client side
- [ ] Add SSL/TLS Certificate for HTTPS
- [ ] More mobile friendly version?

