---
layout: wiki
category: wiki
subcategory: video-games
title: UE Classic FPS Movement Pack
publication: Unreal Engine
link: https://forums.unrealengine.com/t/classic-fps-movement-pack/33083
date: 2025-02-02
---

"Movement is such an underrated part of a FPS game (and potentially a TPS game) that gets often overlooked vs focus on weapon and enemy design. I’ve always found enjoyment in good movement physics, and in my opinion it can make or break the game. You need your player to feel like they are one with their character, so movement needs to be incredibly responsive. With that goal in mind I’ve been working on a movement pack that adds responsive, creative player movement similar to beloved FPS classics.

List of features:

* **100% in blueprint**, so you can easily customize all aspects of the included movement behaviors.
* **Adds true air acceleration/air strafing**. Air control using air acceleration enables techniques such as air strafing, circle jumping and much greater precision and skill ceiling in movement. Fully customizable acceleration values/thresholds. This is really the meat of this movement pack. The best way I can describe air acceleration based air control is that it gives the feel of controlling a finely tuned sports car, whereas non accelerating air control (default in UE4 engine) gives the feeling of driving a boat. Proper air acceleration becomes essential to give precise air control at a variety of speeds. This can be as simple as trying to steer a jump around perilous cliff edges or navigate through a movement puzzle, or as advanced as maintaining precise control while rocket jumping 50mph through a map (see below :P).
* **Adds Ground acceleration** adds additional acceleration when turning, giving a tighter feeling movement while turning on the ground. This is a minor effect that many players probably aren’t aware of in some of their favorite FPS games, but I find it does make a difference in the feeling of responsiveness to general player movement. The presence of ground acceleration also indirectly allows techniques such as strafe jumping- so that you can use certain techniques to start a jump with additional lateral speed.
* **Adds trimping**: Downward and upward ‘trimping’ with separately customizable slope angle thresholds and velocity boosts. What is trimping? Originally I believe this was a quirk in CPMA (quake mod) jump handling that behaved as follows: Downward trimp: Gain some horizontal speed when jumping down ramps at expense of vertical.
* **Upward trimping**: Gain some vertical speed when jumping up ramp at expense of horizontal speed.
* **Adds Rampsliding** seen in games such as quake/halflife/tfc/ff/TF2, etc… Hitting an inclined surface at enough velocity allows you to smoothly glide up it with some steering ability. Customizable minimum angle, minimum speed threshhold (i.e. 2x walk speed) and momentum factors. NOTE: surfing not supported
* **Adds pogo jumping, crouch jumping** - hold space to jump repeatedly if desired, and allow crouch jumping if desired. (default UE4 engine seems to have hard coded no jumping when crouched…so this optionally will fix that). Note: multiplayer pack currently has no crouch jumping implemented
* **Adds bunnyhopping**. Together with air acceleration and optional pogo jumping (hold space to continually jump) bunnyhopping can be unleashed if you so choose. There is a fully customizable cap so you can cap or prevent speed gained but still maintain the benefits of air acceleration. By adjusting the included variables you can apply a soft or hard cap (i.e. 2x walk speed) or none at all.
* **Adds a simple HUD speedometer:**because half the fun may be seeing how fast you can go! Realistically this is just a simple speedometer to help you fine tune movement to your preferences.
* Adds rocket jumping: A simple multiplayer compatible rocket launcher is included for those that want a starting point for how you would implement weapon jumping.

Any of the above features can be independently enabled/disabled. You could choose a low air acceleration and limit players to gain speed only by trimping down ramps and weapon jumping, or you could apply a strong speed cap on bunnyhopping but retain strong air acceleration to allow its creative use in dodging, weapon jumping etc. Or uncap everything and unleash hell (I hope you made a large or procedurally generated map…you quickly run out of real estate travelling at 10000+u/s as I’ve found :P)"
