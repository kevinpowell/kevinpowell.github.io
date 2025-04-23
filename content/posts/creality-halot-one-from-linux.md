+++
date = '2025-04-22T17:10:36-07:00'
draft = false
title = 'Creality Halot One From Linux'
tags = [linux 3dprinting]
+++
This is not much of my original work.  But here goes anyway -- I got a Creality Halot One for cheap
on EBay.  It's not a bad little resin printer.  However, the mfr software (Halot Box) is windows only.
I got a little tired of having to spin up my Windows VM in order to start up a print.  So, I went
looking for linux native options.

git clone https://github.com/danielkucera/creality-remote-control.git

danielkucera has done a fine job with that project -- it is just a little html/javascript that one
loads up in a browser.  The javascript talks to the Halot One, and allows control of the printer (send file,
start, stop).  It is spartan in its design aesthetic, which I like.

So, then one needs to be able to take a model and make a cxdlp that the Halot can print. I went with
the free version of chitubox.  It seems like prusa-slicer in combination with UVTools can also
create the cxdlp files that Halot wants.

Now, I have a full linux-native 3d printing workflow:
    FreeCAD -> .stl export -> chitubox -> cxdlp -> creality-remote-control
