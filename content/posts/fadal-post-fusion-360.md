+++
date = '2025-02-17T17:29:28-08:00'
draft = false
title = 'Fadal Post Processing and Fusion 360'
tags = ["fadal", "cnc", "fusion"]
+++
My fadal VMC20 does not like the nc code that comes out of the default fadal post-processor
in Fusion360.  The g-code interpreter on the machine does not like the generated comments.
Here's my solution:
1. edit the fadal.cps (post definition)
2. find the writeComment function; delete the part that adds the closing paren. Also find the onOpen function and delete the close paren added there (but not using the comment function -- not great programming)
3. voila!

When drip feeding the F360 generated nc programs, use DNC,0,1 (turn off error check)
