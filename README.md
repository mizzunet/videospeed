## Faster HTML5 Video

HTML5 video provides a native API to accelerate playback of any video. The
problem is, many players either hide, or limit this functionality. For best
results playback speed adjustments should be easy and frequent to match the pace
and content being covered: we don't read at a fixed speed, and similarly, we
need an easy way to accelerate the video, slow it down, and quickly rewind the
last point to listen to it a few more times.


\*\* Once the extension is installed simply navigate to any page that offers
HTML5 video ([example](http://www.youtube.com/watch?v=E9FxNzv1Tr8)), and you'll
see a speed indicator in top left corner. Hover over the indicator to reveal the
controls to accelerate, slowdown, and quickly rewind or advance the video. Or,
even better, simply use your keyboard:

### Install
1. Dowload latest release
2. Install it by Addons > Gear icon > Install Addon from File

### Usage

```
S decrease playback speed.
D increase playback speed.
R reset playback speed to 1.0x.
Z rewind video by 10 seconds.
X advance video by 10 seconds.
G toggle between current and user configurable preferred speed.
V show/hide the controller.
```

You can customize and reassign the default shortcut keys in the extensions
settings page, as well as add additional shortcut keys to match your
preferences. For example, you can assign multiple different "preferred speed"
shortcuts with different values, which will allow you to quickly toggle between
your most commonly used speeds. To add a new shortcut, open extension settings
and click "Add New".

![settings Add New shortcut](https://user-images.githubusercontent.com/121805/50726471-50242200-1172-11e9-902f-0e5958387617.jpg)

Some sites may assign other functionality to one of the assigned shortcut keys —
these collisions are inevitable, unfortunately. As a workaround, the extension
listens both for lower and upper case values (i.e. you can use
`Shift-<shortcut>`) if there is other functionality assigned to the lowercase
key. This is not a perfect solution, as some sites may listen to both, but works
most of the time.

### FAQ

**The video controls are not showing up?** This extension is only compatible
with HTML5 video. If you don't see the controls showing up, chances are you are
viewing a Flash video. If you want to confirm, try right-clicking on the video
and inspect the menu: if it mentions flash, then that's the issue. That said,
most sites will fallback to HTML5 if they detect that Flash is not available.
You can try manually disabling Flash from the browser.

**What is this fork of `igrigorik/videospeed` all about?** This fork of the
[`igrigorik/videospeed`](https://github.com/igrigorik/videospeed) repository
is a port of [`igrigorik`](https://github.com/igrigorik)'s videospeed Chrome 
add-on for Firefox. This fork modifies the Chrome add-on code so that it works 
in Firefox. This repo is the code behind the [Firefox Extension](https://addons.mozilla.org/en-us/firefox/addon/videospeed/)
whereas the [`igrigorik/videospeed`](https://github.com/igrigorik/videospeed)
repository contains the code behind the [Chrome Extension](https://chrome.google.com/webstore/detail/video-speed-controller/nffaoalbilbmmfgbnbgppjihopabppdk).

### License

(MIT License) - Copyright (c) 2014 Ilya Grigorik
