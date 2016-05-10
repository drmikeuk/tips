---
layout:     page
title:      "Gimp"
---

[Gimp](https://www.gimp.org/) is a free image editor with similar functionality to Photoshop.

Install
-------

[Download here](https://www.gimp.org/downloads/), and install.  
Then drag to your dock for easy access.

Tips
----

### Resize image

* Image > Scale image

_See the full [Gimp documentation](https://docs.gimp.org/2.8/en/gimp-tutorial-quickie-scale.html)_

### Crop image

* Use the rectangle select tool
	* hold down shift __after__ you have started selecting to force to a square
* Image > Crop to selection
* Resize if required: Image > Scale image (eg 300x300 pixels)
* Save as new file: File > Export as

_See the full [Gimp documentation](https://docs.gimp.org/2.8/en/gimp-tutorial-quickie-crop.html)_

### Darken / lighten image

You can use the [levels](https://docs.gimp.org/en/gimp-tool-levels.html) tool to make an image lighter or darker or to change the contrast.

[See this tutorial](http://www.lpgallery.mb.ca/gimp/g4.htm) with nice "before and after" examples of dark & low contrast photos.


Putting it all together
-----------------------

Aim: take a section of [this 3223×2558 pixel 19th Century map of London](https://www.flickr.com/photos/britishlibrary/11132833506/) and make a 1000x200 pixel pale background image.

![Original map of London](/assets/media/london_small.jpg)  <i class="fa fa-arrow-right fa-2x" aria-hidden="true" style="padding: 10px"></i> ![Final map](/assets/media/london-final.jpg){: style="max-width: 50%;"}

### Outline

1. Select an area of interest using the the rectangle select tool
	* it doesnt matter if this is wider than our target 1000 pixels -- we will resize later
	* make the selection higher than needed -- we will crop this later
1. Crop: Image > Crop to selection
1. Resize to target width: Image > Scale image: 1000 pixels
1. Adjust to target height: Image > Canvas size: Height = 200 pixels (& change offset Y to move selection down if required)
1. Lighten: Tools > Colour tools > Levels: change input levels to 192
1. Save as new file: File > Export as

### Steps

1) Select an area of interest using the the rectangle select tool

* it doesnt matter if this is wider than our target 1000 pixels -- we will resize later
* make the selection higher than needed -- we will crop this later

![Map showing selection](/assets/media/london-select.jpg){:.img-responsive}

2) Crop: Image > Crop to selection

3) Resize to target width: Image > Scale image: width = 1000 pixels

![Cropped map](/assets/media/london-cropped.jpg){:.img-responsive}

4) Adjust to target height: Image > Canvas size: Height = 200 pixels (& change offset Y to move selection down if required)

![Cropped map after changing canvas size](/assets/media/london-canvas.jpg){:.img-responsive}

5) Lighten: Tools > Colour tools > Levels: change input levels to 192

![Levels tool](/assets/media/levels.jpg){:.img-responsive}

![Final map](/assets/media/london-final.jpg){:.img-responsive}

6) Save as new file: File > Export as












