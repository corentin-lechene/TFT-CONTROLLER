# TFT CONTROLLER

I know that my script is not very useful especially since TFT mobile exists. However, I had an urge to play it on my TV with my controller. <br>
The scripts found on the internet did not work or worked badly. So I created this project to allow me to play in my way and to make it open to everyone.<br>

A debugging system is in place to allow you to play even if your screen is atypical. It's simple and will take you a few minutes. (See [Troubleshooting](/README.md#Troubleshooting) → Mouse position wrong))

You can change the configuration as you wish only if it's possible. (See [Planned Hotkeys](/README.md#Planned-Hotkeys))

## How it will work
You will be able to play (finally) with the controller your favorite game deported from your PC / Phone. The directional arrows allow you to move on the ground. All TFT shortcuts have been added and can be modified.
You can use the left joystick to move the mouse in a circle to get your champion or recover items.

### Installation
1. Download and install AutoHotkey from https://www.autohotkey.com/download/
2. Download the Script from my GitHub

### Setup
1. Edit the file in the section ``Configuration`` _(line 25)_ then add your resolution by changing these two values `RESOLUTION_X := 1920` and `RESOLUTION_Y := 1080`
2. Save and run

### Planned Hotkeys
| Key (PS4 - XBOX)    | Function (By default)       | Shortcuts TFT | Editable |
|---------------------|-----------------------------|---------------|----------|
| SQUARE   -  X       | Buy XP                      | f             | Yes      |
| CROSS    -  A       | Left Click                  |               | Yes      |
| CIRCLE   -  B       | Reroll                      | d             | Yes      |
| TRIANGLE -  Y       | Sell                        | e             | Yes      |
| L1       -  LB      | Next board                  | q             | Yes      |
| R1       -  RB      | Previous board              | r             | Yes      |
| L2       -  LT      | Left Click                  |               | Yes      |
| R2       -  RT      | Deploy / Return to bench    | w             | Yes      |
| L1 & R1  -  LB & RB | Your board                  | Space         | Yes      |
| L2 & R2  -  LT & RT | Do nothing                  |               | Yes      |
| Directional arrow   | Left / Right / Down / Up    |               | No       |
| Joystick left       | Mouse the mouse in a circle |               | No       |


### Troubleshooting

| Name of the Troubleshooting | issues                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|-----------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Controller not detected     | Try to change this value `NUM_CONTROLLER := 1` to 2 ou 3...                                                                                                                                                                                                                                                                                                                                                                                           |
| Mouse position wrong        | Change this value `DEBUG := 0` to 1 and then restart the script. You'll see a little window that will follow your mouse. It displays the percentage of your location. <br/>Get the values on each squares and add these values in their corresponding variable.(line 79-90) <br/>**Warn !** Take coordinates like this : <u>Up to Down an Left to Right</u><br/> _Exemple (for shop) :_ ``AREA_SHOP_X := [x1, x2.., x5]`` and ``AREA_SHOP_Y := [y1]`` | 

### Disclaimer

This script was created for me and for others who would like to have the possibility to play with a controller. You can use an XBOX or PS4 controller, I did not test the others.<br>
<u>**Warning :**</u> I'm not responsible if Riot decides to ban you for using a 3rd party app, though I believe it follows their TOS since nothing is being automated or anything, and Autohotkey is used for other LoL stuff I've seen, so I'm not too concerned about using it myself. Hopefully someone finds it at useful.
