# Minor WebDev | Lifely
Dave Bitter | 500710907

    v1.0.0

## General
This repository holds documentation for [Lifely's](https://lifely.nl/) [Fresh Heroes project](https://freshheroes.com/), part of the minor "Webdevelopment" at the [HvA](http://www.hva.nl/)

## What did I focus on?
The website is accessible through traditional inputs like pointers and keyboards. I want to make use of gesture inputs to navigate through the entire site and for other actions that can be enhanced by this. Furthermore, I wanted to add a cool feature that made use of a device's gyroscoop. 

## Initial idea generation
Through quickly sketching idea's I came up with a few idea's to build. I didn't build all of the idea's due to time constraints and generally purposfulness (e.g. rotate gesture to go through browser history). You can view the initial idea's below.

### Initial idea's
![initial idea's](https://raw.githubusercontent.com/DaveBitter/minor-webdev_lifely/develop/images/idea_0.png)
![initial idea's](https://raw.githubusercontent.com/DaveBitter/minor-webdev_lifely/develop/images/idea_1.png)
![initial idea's](https://raw.githubusercontent.com/DaveBitter/minor-webdev_lifely/develop/images/idea_2.png)

## Library research
I wanted to find a good libary to make us of for the functionalities although I could make use of the Javascript touch events. Again, due to time constraints this is the fastest and most reliable way since I could'nt test thoroughly. 

### Found Libraries
I initially found three candidates:
* [Zingtouch](https://www.npmjs.com/package/zingtouch)
* [Hammer.js](https://www.npmjs.com/package/hammerjs)
* [InteractJS](https://www.npmjs.com/package/interactjs)

### Chosen library
At first, I chose for Zingtouch. It seemed to be the most well documentend one of the three. I quickly discovered a deal-breaker. Zingtouch handles [this issue](https://www.chromestatus.com/features/5093566007214080) very poorly. Next in line was the most popular, based on downloads, of the list. Hammer.js does the job and does the job good. Therefor, I used this library the rest of the project.

## Build functionalities
During this project I focussed on three area's. Using gestures to navigate, using gestures to discover and using the device's gyroscoop.

### Gesture based navigating
Firstly, a user can now swipe in from the side to open the mobile menu. This is intuitive since this is default behaviour in a lot of apps. 

Secondly, a user can now swipe the header to navigate through the main 3 pages. This allows for quick navigating through the main pages.

Finally, the most useful of the three. A user can now swipe to the next or previous vacancy on the detail vacancy pages. Previously, you had to go back to the oveview page and click the next vacancy. This will improve usability and efficiancy greatly.

![gesture based navigating](https://raw.githubusercontent.com/DaveBitter/minor-webdev_lifely/develop/images/screenshot_0.png)
![gesture based navigating](https://raw.githubusercontent.com/DaveBitter/minor-webdev_lifely/develop/images/screenshot_1.png)

### Gesture based discovery
A user can now pinch out on an image of a internship supervisor in order to see a larger photo and the social links for that supervisor. THis functionality gives the user more information about the supervisor which is useful. When a user pinches back in, the image return to it's original size and the social links are hidden again.

![gesture based discovery](https://raw.githubusercontent.com/DaveBitter/minor-webdev_lifely/develop/images/screenshot_2.png)
![gesture based discovery](https://raw.githubusercontent.com/DaveBitter/minor-webdev_lifely/develop/images/screenshot_3.png)