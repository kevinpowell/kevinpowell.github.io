+++
date = '2025-02-17T16:13:05-08:00'
draft = true
title = 'Usb C Dock Audio'
tags = ["linux", "audio"]
+++
I upgraded my audio setup at my desk by adding a new amplifier (ZK AS21) and nice speakers.
Tried out the amp with my phone as a source and everything sounded great.  Unfortunately, when
using my USB-C dock with onboard KTMicro (KT_USB_AUDIO) audio things sounded terrible: buzzing,
weird hooting noises, etc.  At first I thought it was a ground-loop problem but adding ground isolation
didn't fix things.  What did help was adding a circuit in-line between the dock and the amp to reduce the
impedance seen by the dock.  As far as I can tell, the dock's 3.5mm TRRS output is optimized for headphones
and things go poorly with a high impedance amp connected there.  Also, the amp wants stereo 3.5mm in (TRS)
while the dock has TRRS (with mic) out -- so I got a splitter from Amazon to do the TRRS -> TRS conversion.
[Headphone to Line-In]https://www.vwlowen.co.uk/radio/headphone2linein/headphones.htm
