---
layout: posts
title:  "Setting up the JoyToKey Key Mapper"
date:   2025-04-09 17:00:00 -0500
categories: About
---

This post guides you setting up the JoyToKey key mapper application for the Copilot.

*Please note: Setting up the JoyToKey application is very easy - this post is detailed only to be sure that set up of the JoyToKey application goes smoothly.*

**Overview of Copilot Key Mapping**

The *Mandelbulb3D Animation Copilot* is a helper tool-set for creating Mandelbulb3D animations. This is done by mapping a game controller and the keys of a standard PC keyboard to the Mandelbulb3D application's Navigator step and angle keys, and recording those keyframe movements to a local database. This gives you a record of the movements of each keyframe of an animation sequence. To accomplish this, a key mapper is needed for which JoyToKey was selected.

You can read more about the JoyToKey key mapper at its <a href="https://joytokey.net/en" target="_blank">website</a>. As as it pertains to the Copilot, the JoyToKey key mapper enables the Copilot to cause the Mandelbulb3D application's Navigator to perform movements in your Mandelbulb3D scene.

For example, when using a game controller as shown below, the JoyToKey application "re-maps" the controller's front right trigger button to the "w" key which the Mandelbulb3D's Navigator recognizes as Walk Forward. The controller's front left trigger button is mapped to the "s" key which the Mandelbulb3D's Navigator recognizes as Walk Reverse.

Another example, when using a game controller the JoyToKey application "re-maps" the "A" button to the cause the Mandelbulb3D's Navigator to create a new keyframe the same as if you were to click the "Ani Key" button on the Navigator window.

<img src="/assets/images/xbox-controller.jpg" width="300">

The JoyToKey key mapper also re-maps the keys of a standard PC keyboard as shown below.

When using a PC keyboard the JoyToKey application passes the movement keys to the Mandelbulb3D's that the Navigator recognizes, and also maps keyboard keys for other functions, such as the "Ani Key" mentioned above that causes a new keyframe to be made.

<img src="/assets/images/Desktop Keyboard Legend.jpg" width="300">

As you can see by the above explanations, the Copilot requires key mapping. As such, the JoyToKey application must be installed and running to be able to use the Copilot alongside the Mandelbulb3D application.

As an aside, both the game controller and PC keyboard legends, as shown above, can be displayed while using the Copilot by clicking the "Show Key Legend" button.

**Obtaining the JoyToKey Application**

We don't want to repeat downloading and installation instructions here. Please visit the JoyToKey  <a href="https://joytokey.net/en" target="_blank">website</a> to download it and for installation instructions. Installation is actually very simple.

We would like to point out to use care that you download the JoyToKey application from its authorized <a href="https://joytokey.net/en" target="_blank">website</a>, being careful to not download from a site that aggregates software downloading that may fool you to download some other software application that you don't want or expect.

*Be sure to download only from the JoyToKey authorized website at <a href="https://joytokey.net/en" target="_blank">https://joytokey.net/en</a>*

At the time of this post, the JoyToKey application is provided as a free or a paid version. *The Copilot works fine with the free version.* However, you may prefer to purchase the paid version given it's additional features and very low price. At the time of this post, the JoyToKey application is a perpetual license, not subscription based.

After the JoyToKey is downloaded and installed on the PC or laptop that you are running both the Copilot and the Mandelbulb3D applications, you **must** configure JoyToKey to use the Copilot's mapping configuration, which is discussed following.

**Configuring the JoyToKey Application for the Copilot**

The file that configures the JoyToKey application to map a game controller and PC keyboard keys for the Copilot can be found in the folder where the Copilot is installed. That file is named *MB3D_JoyToKey.cfg* as highlighted in the image below.

<img src="/assets/images/Location of JoyToKey Config File.jpg">

Note: The installation folder for the Copilot will normally be located in the "Mandelbulb3D Animation Copilot" sub-folder of the Windows "Program Files" folder.

The *MB3D_JoyToKey.cfg* is a file that must be loaded into the JoyToKey application for purposes of the Copilot. The process is actually very simple.

1. Stop and exit the JoyToKey application.
2. Copy (don't cut) the *MB3D_JoyToKey.cfg* file from the Copilot installation folder to the installation folder of JoyToKey (which is normally in your Windows Documents folder).
3. With *MB3D_JoyToKey.cfg* pasted in JoyToKey's folder, delete the file *Profile 1.cfg* in the JoyToKey folder. The file may be named "default.cfg". You only want one .cfg file in the folder, which should be the *MB3D_JoyToKey.cfg* file.

<img src="/assets/images/JoyToKey Config Folder with Copilt file highlight.jpg">

With the files taken care of, restart the JoyToKey application and open it's interface. In the window's title you should see that the *MB3D_JoyToKey* configuration is now in use by the JoyToKey application. The JoyToKey interface should look like below (the dark theme is shown here).

<img src="/assets/images/JoyToKey Interface with Copilot cfg.jpg">

*Please note: You do not need to do anything else with the JoyToKey application once the MB3D_JoyToKey configuration is loaded.*

With the *MB3D_JoyToKey* configuration set up, you have the ability to use a game controller or your PC or laptop keyboard while using the Copilot to navigate your Mandelbulb3D scene.

Thank you for using the Mandelbulb3D Animation Copilot!