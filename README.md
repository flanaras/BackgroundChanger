# background-changer

This is an application that changes the desktop background from a given set of images using some pattern.

1. parse folder set for images
2. run a timer 

The desktop's wallpaper will be set to the one that is closest to the last year's date.

## Examples

### First example of the pictures rotation

struct data [date (with or without year), time]

struct data images -> a, b, c, desktop, now

**a** < **now** < **b** < **c**

The image will be set to **a**

When **b** <= **now** < **c** it will change to **b**

### Second example

Rotate picture every x minutes, in a sequence or in random order.

### Third example 

Rotate location based. Provide an area/country/city and take only those pictures.

## Supported platforms

Initially this projects will be supported on the following Operating Systems.

* Windows
* Linux/Gnome 3
