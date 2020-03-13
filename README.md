# py-ambi-light

This is currently a placeholder for a future project I am planing.

I hope to build an ambi-light device with a Raspberry Pi, and Pi Camera, and some neopixels.

The idea is that the camera will in some way sense it's environment 
(such as proximity of a moving object, or sensing specific colours in an object) 
and respond to that input by changing a pattern/colour on the NeoPixels.

The overall effect will be a sort of 'mood light' that is inactive when the room is empty,
but when someone walks past it, it slowly starts to respond with different colour patterns
in an attempt to keep the person neary for longer (triggering surprise and intreague!)

I am hoping to build the application in two parts, a set of device drivers/generic maths
that can be used to sense and control, and a separate 'hole' in the code that others
can write their own mini applications in order to achieve specific (and different) effects,
thus turning this into a reusable platform for artists to further innovate on top of.

David Whale

March 2020
