Post-Processing Utilities
=========================

This repository contains some small utility scripts for
[the post-processing stack][PostProcessing].

PostProcessingController
------------------------

**PostProcessingController** provides a simple interface to modify the settings
of the post-processing stack. It exposes all the settings and enable/disable
flags as public members. These members can be directly modified from the
inspector, scripts and animations.

![inspector](http://i.imgur.com/7cFoof1m.png)
![animation](http://i.imgur.com/YRuF7nAl.png)

It creates a clone of the profile when starting the Play mode, and thus it can
avoid modifying the profile asset with changes. This is similar to
[`Renderer.material`][RendererMaterial] that automatically creates a clone of
a material on changes.

FocusPuller
-----------

**FocusPuller** automatically updates the focus distance of the depth of field
effect depending on the distance from the camera to a target object.

![gif](https://67.media.tumblr.com/9843254db0c0b00255bb769c93e506e3/tumblr_ogoay0yY0p1qio469o1_320.gif)
![gif](https://66.media.tumblr.com/58b49719b9bdde6c480b8abdba2571ab/tumblr_ogoay0yY0p1qio469o2_320.gif)

It uses PostProcessingController to update the distance value dynamically.

How To Use
----------

Download and import [the unitypackage file][Unitypackage]. That's it :smiley:

[PostProcessing]: https://github.com/Unity-Technologies/PostProcessing
[RendererMaterial]: https://docs.unity3d.com/ScriptReference/Renderer-material.html
[Unitypackage]: https://github.com/keijiro/PostProcessingUtilities/blob/master/PostProcessingUtilities.unitypackage
