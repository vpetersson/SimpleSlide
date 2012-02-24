## About SimpleSlide
SimpleSlide is a proof-of-concept that was developed for a client that wanted to run a projector in his store-front to display advertisement. Yet he did not want to constantly have to rebuild the slide deck by hand. SimpleSlide solved his problem.

## How It Works
SimpleSlide runs on a dedicated Mac (a Mac Mini works great) with one or several screens connected. The Mac has a network share that is accessible on the local network. In order to create a slide show, the users simply drag and drops a set of images into the network share. Once the user has dropped the image files in the share, the following happens:

* SimpleSlide takes the images from the shared folder and resizes them into the desired resolution (configurable in the source code).
* Next it launches Apple Keynote and creates a slide show with the right settings (resolution etc).
* Once the slide show is created, it then takes all the images and adds them into the presentation on separate slides as well as setting the correct properties (transition, time interval etc.)
* SimpleSlide then runs the presentation x times and then goes back to the beginning where it looks for changes in the network share (added or removed images) and starts over. X is configurable in the source code. 


## Requirements

* Mac OS X Leopard
* Apple iWork '08 or later


## Installation
Run the install application in the packages and follow the directions.

## License
SimpleSlide is released under [GPLv3](http://www.opensource.org/licenses/gpl-3.0.html).

## Demo
View [demo on YouTube](http://www.youtube.com/watch?v=YHx3lWuPFTE).

## Known bugs
See the [Issues-section](http://github.com/vpetersson/SimpleSlide/issues/) .


## Feedback and contribution
I greatly appreciate feedback and contributions to SimpleSlide. If you have any changes or feedback, please drop me a line or submit your contribution directly to Github.

## Simple Slide has been discontinued
I won't spend any time on developing SimpleSlide further as it has been discontinued. The primary reason is because I developed a completely new software for [Skärmverket](http://skarmverket.se/) that is more stable, runs on Linux, and is built from the ground up to be run and managed remotely.

That said, the source code for SimpleSlide is available, and you are free to use it. Just don't expect any bug fixes.