---
layout: posts
title:  "Copilot Movement Actions"
date:   2025-04-09 16:00:00 -0500
categories: About
---

This post explains the movement actions used by the Copilot.

**Movement Structure**

The structure of a movement action is as follows:

[MOVE NAME][MOVE COUNT] (STEPS or ANGLE)

Examples:<br>
"WF1 (500)" translates to Walk Forward one time with a step count of 500 for each walk forward.<br><br>
"LD3 (5)" translates to Look Down three times with an angle of 5 for each Look Down.<br><br>
"SR5 (5)" translates to Slide Right five times with step count of 5 for each slide right.

**Movement Names**

Each move action has an abbreviated name, for example "WF" means "Walk Forward". Below is a list of each of the possible move action abbreviations and the meaning for each.

*Walking*<br>
WF = Walk Forward<br>
WR = Walk Reverse<br>

*Looking*<br>
LR = Look Right<br>
LL = Look Left<br>
LU = Look Up<br>
LD = Look Down

*Sliding*<br>
SR = Slide Right<br>
SL = Slide Left<br>
SU = Slide Up<br>
SD = Slide Down<br>

*Rolling*<br>
RCW = Roll Clockwise<br>
RCC = Roll Counter-Clockwise

**Multiple Movements**

There can, and usually are, multiple movement actions per keyframe. The following is an example of two movement actions for a keyframe:<br><br>
WF1 (500) LD3 (5)

While no limit to the number of moves of a keyframe is imposed by the Copilot, there are only a certain number of movement actions that can be made for a keyframe. The following is an example of 4 movement actions for a keyframe:<br><br>
WF1 (500) LD1(5) LR1(5) RCC2(5)

You can see by the above movement set that the keyframe movement was Walk Forward once (WF1), Look Down once (LD1), Look Down once (LD1) and Roll Counter-clockwise twice (RCC2). This is a fairly complex movement that, along with other keyframe movements, can make for very interesting animation sequences. 

Below is a graphic of a list of movement actions that were part of a 316 keyframe animation. Each row represents a keyframe with the movements associated with that keyframe.

<img src="/assets/images/Copilot_Keyframe_Stack.jpg" width="450">

**Movement Tracking**

With the information presented in this post, you should now understand the movement nomenclature used by the Copilot. This is important because while you are animating, the movement actions are displayed on the screen to give you a visual of what movements are occurring, as the screenshot below shows.

<img src="/assets/images/Screenshot Copilot Making Movements.jpg">

An important purpose of the Copilot is to record movement actions of each keyframe to help you create realistic movements through your Mandelbulb scene. As you navigate through your scene, the Copilot "stacks" the movements of each keyframe at the top of the "Keyframe Stack". This allows you to quickly review the movement or movements that went into keyframes that preceed the keyframe you are working on.

An important goal of the Copilot is to help you create animations with movements that are well coordinated throughout the animation. If you can "see" where you've been in your animation, you have a much better chance of keeping your animation well coordinated. In addition, you are less likely to create animations that have distracting and unrealistic movements. You are also much less likely to have to start your animation keyframes from the very start because your animation didn't turn out well that perhaps you only discovered after a lengthy render of your animation frames.

*Keep Creating!*