## Interface Guidelines

While the OUYA platform is as open as possible, we realize that some semblance of structure can be a good thing.

Whether you’re writing a new game exclusively for OUYA, or porting an existing one, your users will thank you if you take the time to engineer a seamless and intuitive experience!


### Button Functions

We recommend the button mappings below. These mappings are legit. Seriously, we’ve explored all types of mappings and these tend to be the most intuitive.

OUYA           |  Color  |  Function          |  Image
---------------|---------|--------------------|----------
O              | green   |  select            |<img src=”http://i.imgur.com/Izzg6f9.png”>
U              | blue    |  -                 |<img src=”http://i.imgur.com/cGndvxa.png”>
Y              | yellow  |  -                 |<img src=”http://i.imgur.com/Izzg6f9.png”>
A              | red     |  back/cancel       |<img src=”http://i.imgur.com/cBffscc.png”>
The OUYA Button| black   |  pause             |<img src=”http://i.imgur.com/0FAl9Io.png”>

### Button Naming

Please use the naming conventions below when referring to the controller buttons in help screens for your game:

```text
O, U, Y, A
The OUYA Button
D-Pad 
LS (the left joystick movement)
L1 (the left bumper)
L2 (the left trigger)
L3 (the button function of pressing the left joystick straight down)
RS
R1
R2
R3
Touchpad (*not* "Trackpad")
```



### Menu Navigation

When porting touchscreen android games to OUYA, adapting menus properly to controller capable navigation can help make your game feel more like a native console game, and reduce user frustration at the same time.

##### Cursor-based Menu Navigation

<img src=”http://i.imgur.com/fDZwrIf.png”>

Forcing the user to navigate your menus (or worse, your game) exclusively with the touchpad is not recommended. Most users will not guess this is what they are supposed to do, and even if they do, they will tire of it quickly. Some users may even be using a third party controller that lacks a touchpad, and will be unable to play your game at all.

##### Action Button Menu Navigation

<img src=”http://i.imgur.com/a4kkb4u.png”>

Many developers porting from a touchscreen platform choose to use this method as it requires less extensive artwork changes. (We even [provide images](https://d31pno3ktcq63f.cloudfront.net/assets/OUYA_Buttons.zip) of the button faces for your use). While this seems like a good compromise, some users may become confused or frustrated because this is not a common method of menu navigation on existing consoles.

##### D-pad/Thumbstick Menu Navigation

<img src=”http://i.imgur.com/9iKi9QQ.png”>

By far your best option is the classic stack-of-words menu, with a highlight or some other effect applied to the selected item, the "O" button being used to confirm the user's selection and the "A" button being used to go back a menu, or quit the game if at the main menu.

Sometimes an existing touch screen menu can be adapted to this method by applying a highlight to existing touch-activated buttons, but care should be taken to make the highlight *very* obvious, and to make sure a default button is highlighted when the menu loads.

To keep even more of your users happy, make sure that both the D-pad *and* the thumbsticks can be used to navigate your menus.

### The Touchpad

We recommend that the only way you utilize the touchpad in your games is for gesture-based input, with the cursor disabled (coming soon!).

An example would be asking the user to swipe upwards on the touchpad to cause their character to perform a special attack, or swipe left to right to bring up a HUD.

<img src=”http://i.imgur.com/jGgBd01.gif">

### Fonts and Text Sizes

Text displayed on a television screen must be larger than on a mobile device in order to be read clearly by all users. This means that less text can be displayed at a time, and that your users will want to be reading less text overall. For longer sections of text, consider voiceovers instead, or spread the text over several screens.

### Sound

Unlike on a mobile device where the user may have the sound muted, or be wearing headphones, on OUYA sound will be coming out of the TV or a stereo system at a higher volume. Test how your sounds and music will sound on as many TVs as possible, and considering replacing any that aren't up to snuff.

### TV Safe Area

Leave at least a 10% margin between your UI elements and the edge of the screen. This will help ensure that your content is visible across a wide range of TVs and settings.

At 1080p, resolution is 1920x1080, so important game elements should be kept inside a centered box of the size 1728x972. That's 96 pixels of margin on the left and right sides, and 54 pixels of margin on the top and bottom.

At 720p, resolution is 1280x720, so important game elements should be kept inside a centered box of the size 1152x648. That's 64 pixels of margin on the left and right sides, and 36 pixels of margin on the top and bottom.

### Testing Environment

Many of the above suggestions become obvious when playing on an actual OUYA on a television. If possible, test your game on an OUYA on a typical consumer television set, not a computer monitor. If you can test with multiple TVs, even better, as different manufactures perform different corrections to the input image.

If your licensing allows for it, consider using the OUYA community to help test your game. Not only will you generate buzz earlier in the development process, but you may gain valuable insight into how users experience your game.