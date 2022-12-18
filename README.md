# WHY ??

Because bCNC interface on 7" touchscreen is not very easy to use.....
So Big Buttons are better ;)



# bCNC-Streamdeck
Based on this excellent interface for CNCjs : [Stream Deck and mobile web pendant for cncjs](https://github.com/Billiam/cncjs-pendant-streamdeck/)



![Stream Deck device with buttons with buttons for CNC ](https://i.imgur.com/zDZwKnU.jpg%5B)
![Stream Deck device with buttons with buttons for CNC ](https://i.imgur.com/rtAGxuj.jpg)
![Stream Deck device with buttons with buttons for CNC ](https://i.imgur.com/0SAgXLg.jpg)
![Stream Deck device with buttons with buttons for CNC ](https://i.imgur.com/5R0FAId.jpg)
![Stream Deck device with buttons with buttons for CNC ](https://i.imgur.com/FoI7eFe.png)

## Compatibility

This has been tested with Python 3.10, Grbl 1.1h, bCNC under Linux, Raspbian and Windows 10 and on RaspBerry PI 3A+ and PI4

## MY HARDWARE

CNC home made with arduino (GRBL 1.1H), raspberry pi 4, 7" touchscreen


## Installation

First : install BCNC if you didn't ! [get bCNC](https://github.com/vlachoudis/bCNC)

[get zip file ](https://github.com/metropolicon/bCNC-Streamdeck/archive/refs/heads/main.zip) 

unzip into bCNC directory ( for exemple into : c:\Python310\Lib\site-packages\bCNC )

only two original files are overwritten....

__main__.py  : integration of streamdeck

sender.py : correction of cpu core overloaded during running or pause ([see my issue in bCNC github](https://github.com/vlachoudis/bCNC/issues/1765))

## FIRST LAUNCH
before launching, you must set the gcodes directory in streamdeck\streamdeck.json

"gcodespath": "YOUR GCODE DIRECTORY"

## LAUNCH
launch bCNC as usually .... (python -m bCNC or your other command )

## DOCUMENTATION
later, i'll can make a tutorial for options and commands....

## LAST UPDATE (2022-12-18)

Bug corrections
Add move to mouse click position (see in streamdeck.json , the 'gotomouse' button )
Add probe zxy macro with enter tool diameter....( see the 'probe_zxy' button )

enjoy ;)
