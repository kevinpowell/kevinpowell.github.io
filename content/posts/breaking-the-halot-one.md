+++
date = '2025-04-22T20:34:11-07:00'
draft = false
title = 'Breaking the Halot One'
tags = ["3dprinting"]
+++
This is not so much "something I made work" and it is more of "I was a dolt and eventually sort of recovered."
My Halot One resin printer lives out in the workshop, and it got knocked while I was working on
a different project.  Resin spilled out of the tank and into the upper area of the printer. Sadly,
I didn't notice right away.  When I did notice, it looked like a relatively small spill -- so I cleaned
up the surfaces, but didn't do any disassembly.

Next time I tried to use the Halot One, it was very unhappy.  Nothing printed, and the print platform
wound up stuck all the way at the bottom.  I figured the z axis motor was toast and started ordering
parts.  Later, I decided to have a closer look.  I took everything apart and found that some resin had
trickled down through the z-motor mounting hole.  I cleaned out the electronics bay and removed the z-motor.
The motor wouldn't turn, so I decided to take it apart, too.

Turns out, resin had gotten into the top bearing of the stepper and frozen the bearing.  The rest of the
motor seemed fine.  So, I think I could have repaired the printer for about $1: the bearings in the
stepper motor are a very common size that is often used on skateboards and you can get 10 for $10 on
Amazon (the specific bearing for the Halot One z-motor is 625z 5x16x5 mm).  Unfortunately, I'd already ordered a whole new motor -- I guess now I have a spare? and plenty of spare bearings, too?

Of course, the whole side-project could have been avoided if I'd not spilled the resin, or if I'd made the
effort to disassemble and clean everything sooner.

Update: more screwing around

Replacing the bearing in that motor was less easy than anticipated.  I got the bearing cocked in its recess
in the aluminum motor housing, and eventually just ruined it.  So, those bearings can be replaced but care
is needed (and make sure you get the wavy washers back in the right spot).

My replacement motor arrived shortly after I'd mangled the original motor, but when I plugged in the replacement,
it didn't turn when the printer was powered on.  Instead it made a horrible buzzing noise and sort of shuddered
back and forth.  I swapped the middle two wires in the stepper harness, and that fixed things.  The part number
on the new motor matched the old one -- but maybe Creality has two subtly different motors with the same part
number?

Also, resin had gotten in between the lcd screen and the glass behind it.  Ebay provided a replacement LCD
assembly (cheap, too).

Having torn the whole thing apart a couple of times, I did finally manage to get the Halot One back together
and working well.  I'm actually impressed with the degree to which it is user serviceable.
