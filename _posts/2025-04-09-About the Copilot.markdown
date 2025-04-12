---
layout: posts
title:  "About the Mandelbulb3D Animation Copilot"
date:   2025-04-09 11:00:00 -0500
categories: About
---
4/9/2025 

**Summary Overview of the Copilot**

The *Mandelbulb3D Animation Copilot* is a helper toolset for creating Mandelbulb3D animations. This is done by mapping a game controller or the keys of a standard PC keyboard to the Mandelbulb3D application's Navigator step and angle keys, and recording those keyframe movements to a local database. This gives the animation creator a record of the movements of each keyframe of an animation sequence.

<img src="/assets/images/MB3D Copilot Main Tab.jpg">

**Introduction to the Copilot**

As described above, the *Mandelbulb3D Animation Copilot* facilitates creating Mandelbulb3D animations by mapping a game controller or the keys of a standard PC keyboard to the Mandelbulb3D application's Navigator step and angle keys and recording those keyframe movements to a local database.

The Mandelbulb3D fractal generator application (shown below) itself does not provide a recording of the movements of keyframes - it only captures the graphical result of an X, Y and Z position of the camera in the scene itself, which becomes a keyframe. During rendering of the animation sequence, the Mandelbulb3D application interpolates the frames between keyframes, which becomes an animation sequence when imported into a video editor. While the keyframe interpolation works very well, the challenge is creating an animation that has realistic movements, which is entirely up to the animation creator.

<img src="/assets/images/Mandelbulb3D_Application.jpg" width="600">

Because the Mandelbulb3D application does not record the movements that results in keyframes, the animation creator has to try to remember the previous keyframe movements when deciding what the movement of the next keyframe should be. If the creator forgets what the previous keyframe movements were, the movements of the resulting animation are likely to look unrealistic in the final rendered animation. This is countered by keeping Mandelbulb3D animations short or keeping movements simple (such as a straight-line flythrough). Or the creator of an animation accepts discarding a faulty animation sequence, perhaps after a lengthy render, and creating the animation keframes over from the start.

The Copilot provides the animation creator with a record of all of the keyframe movements of an animation project, which in turn facilitates complex or long animation sequences with a realistic movement flow. The premise of the Copilot is to help the animation creator keep track of the movements of previous keyframes to help determine subsequent keyframe movements. The overall objective is to facilitate animations with realistic movements, and even long or complex animation sequences.

<img src="/assets/images/Mandelbulb3D_Animator_Keyframes.jpg" width="500">

**Primary Objective of the Copilot**

The primary objective of the Mandelbulb Animation Copilot is to record the step and angle movements of each keyframe of a Mandelbulb3D animation sequence, storing those movements in a sqlite database local to the Copilot installation. This assists creators making animations that are realistic in movement primarily because the creator knows the movements of preceding keyframes.

For instance: assuming that keyframe #1 consisted of a walk forward of 5 steps, the animation creator would assume that a movement for keyframe #2 of a walk forward 5 steps would result in a realistic straight-line movement with a consistent speed. In this example, the Copilot would record to its database a "WF5" for keyframe #1 and a "WF5" for keyframe #2.

Taking this example a bit further, let's assume that the animation creator wants to walk forward for 6 keyframes and then begin a right-hand turn with a look-right movement. The animation sequence would look like this: WF5, WF5, WF5, WF5, WF5, WF5, LR1.

So far, the movements of these 7 keyframes are easy to remember. But when the creator is further along in the number of keyframes it get hard to remember what movements have occurred in prior keyframes. That's when an animation sequence starts to get hard to continue making while trying to avoid movements that are visually awkward such as a sudden jerk to the right.

The Copilot addresses the lack keyframe movement recording by the Mandelbulb3D application. The Mandelbulb3D application does not record the steps and angle of the movements of keyframes - it only graphical records the position of the camera in the scene. These scene positions become the keyframes that the Mandelbulb3D interpolates to create an animation. However, the actual movements of each keyframe are not stored which makes creating longer and complex animations challenging.

For example, if the creator were getting ready to make keyframe #33, without aid she has to remember what movements occurred in the previous 32 keyframes in order to continue a realistic animation sequence. The Copilot records the movements of each keyframe to facilitate the creation of long and complex animations using the Mandelbulb3D application. In this example, the creator is aware of the movements of the preceding 32 keyframes and can make an informed decision for the movement of keyframe #33 and beyond.

**Movement Control**

A core function of the Copilot is to record the movements that occurred for each keyframe, for example a walk-forward, a look-left, a slide-down, to site a few movement examples. The recording of movements is key to creating animation sequences that are visually appealing. However, it is difficult to create longer or complex animations using only a PC keyboard. The reason for that is simple; the creator tends to lose the sense of the movement between the time of one keyframe movement to the next. To address this the Copilot adopts the hand-held video console game controller to assist creating animations with the Mandelbulb3D fractal generator application.

The game controller is designed for intuitive hand-held control of movement along the X, Y and Z coordinates in a video game three-dimensional scene. The same X, Y and Z coordinates apply in a Mandelbulb3D scene as well, making the game controller a perfect hand-held device for creating Mandelbulb3D animation. In addition, a game controller reduces the time between keyframes to mere seconds which allows the creator to maintain a sense of movement through the Mandelbulb3D scene rather than be slowed and interrupted by keyboard key presses.

With the Copilot the joysticks and buttons of the game controller are mapped to the keyboard keys that the Mandelbulb3D application's Navigator recognizes. For instance, the controller's right trigger is mapped to Mandelbulb3D's "e" key, which is Mandlebulb3D's command to walk one step forward. The controller's left trigger is mapped to Mandelbulb3D's "s" key, which is Mandlebulb3D's command to walk one step in reverse. As such, the creator can walk forward one step simply by actuating the controller's right trigger, and walk in reverse with the controller's left trigger.

<img src="/assets/images/xbox-controller.jpg" width="300">

By utilizing the game controller for creating Mandelbulb3D animations, the creator can move through the scene using a hand-held device that responds quickly, is intuitive, virtually eliminates interacting with the PC keyboard (which saves time) and makes creating Mandelbulb3D animations much more enjoyable. Perhaps the best benefit of a game controller for Mandelbulb3D animation creation is how rapidly one can keyframe an animation sequence, in addition to the intuitive control of the X, Y and Z movement through the scene.

While long animations are not the primary objective of the Copilot, long animations are well within reach given movement aids such as the game controller. Animations that span several minutes provide a more complete presentation than short animations and can be more immersive for viewers. Being able to produce 50, 100 or more keyframes in a much shorter period of time than without a game controller is great. But the controller becomes essential for animations that involve complex movements, such as the example shown below of a portion of of a 316 keyframe sequence. This is because the game controller provides movement control that is intuitive and rapid that, in turn, helps maintain the creator's movement plan for the animation.

<img src="/assets/images/Copilot_Keyframe_Stack.jpg" width="450">

**Repeating Movements**

One of the characteristics of an animation, basically any animation, is that it contains movements that repeat. For instance, moving forward for each of 10 keyframes, in the case of a Mandelbulb3D animation, would entail 1 step forward for each of the 10 keyframes. That means the creator did one step forward, made a keyframe, did another step forward, made a keyframe, and so on. Very repetitive. But reputation is important in an animation to maintain a steady speed or perform a realistic turn, as two examples.

Using the Copilot there are two methods to perform repetitive step sequences. Let's use the walk-forward step that has the nomenclature of "WF" with the number indicating the number of steps. So, "WF1" is walk forward 1 step, WF5 is walk forward 5 steps, WF10 is 10 steps, and so on.

One step forward for each of 10 keyframes, e.g., WF1, WF1, WF1, WF1, WF1, WF1, WF1, WF1, WF1, WF1 or
10 steps forward for one keyframe, e.g., WF10
#2 above is much easier to implement, but not always the best choice. Let's assume, for example, that you needed to move according to #1 above. That get's laborious. But the Copilot provides the ability to pre-design move sequences. In this example you could have a move sequence named "Move Forward 1 step for 10 keyframe". When you select that "Step Sequence" the Copilot performs all of the moves of the selected sequence, including causing the Mandelbulb3D Navigator to perform the moves, adding the keyframes to the Animation window and storing the moves in the Copilot's database. You did nothing nut select your pre-designed move sequence!

Another capability of the Copilot allows you to repeat all of the moves of a previous keyframe. For instance, let's say you made the following moves in keyframe #45: WF2, LR2, SR1, and RCC2. If you want the Copilot to repeat those exact same moves for the next keyframe (#46 in this example), you simple press "Y" on your controller (or "B" on the keyboard) and the Copilot repeats those moves including causing the Mandelbulb3D Navigator to perform the moves, adding the new keyframe to the Animation window and storing the moves in the Copilot's database.

The goal of pre-designed movement sequences and repeating the last keyframe moves is to give the creator tools to perform repetitive and complex movements easily, with perfect replication and with less mistakes. These capabilities of the Copilot also make creating animations less laborious (more enjoyable) and facilitate venturing into long and complex animations to be proud of.

*Keep Creating!*