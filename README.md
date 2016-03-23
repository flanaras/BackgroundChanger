# background-changer

This is an application that changes the desktop background from a given set of images using some pattern.

1. parse folder set for images
2. run a timer and load next image

The desktop's wallpaper will be set to the one that is closest to the last year's date.

## Requirements

### General:

* Whenever the user logs in there is going to be a process that will listen and do any changes set by the user
* Somehow there is going to be a "settings panel" that will be easy accessibility

#### Windows:

* There is going to be a task on the start-up apps to run the daemon.
* There is going to be an entry while right clicking on the desktop which will show options and load next image.

#### Linux/Gnome:

* A Gnome extension is going to provide the options panel

## Examples

### First example of the pictures rotation

struct data [date (with or without year), time]

struct data images -> a, b, c, desktop, now

**a** < **now** < **b** < **c**

The image will be set to **a**

When **b** <= **now** < **c** it will change to **b**

### Second example

Rotate picture every x minutes, in sequence or in random order.

### Third example 

Rotate location based. Provide an area/country/city and take only those pictures.

## Supported platforms

Initially this projects will be tested and supported on the following Operating Systems:

* Windows \[8.1 or/and 10\]
* Linux/Gnome \[openSUSE\]
