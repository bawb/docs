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

### TV Safe Area

Leave at least a 10% margin between your UI elements and the edge of the screen. This will help ensure that your content is visible across a wide range of TVs and settings.

For further tips and advice, read [Google's Designing for TV Guide](https://developers.google.com/tv/web/docs/optimization_guide).