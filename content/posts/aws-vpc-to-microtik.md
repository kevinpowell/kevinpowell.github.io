+++
date = '2025-06-17T10:27:13-07:00'
draft = false
title = 'Aws Vpc to Microtik Site-to-Site VPN'
tags = ['AWS', 'microtik']
+++
I wanted to have the company's AWS vpc accessible directly from the office LAN, without
exposing the EC2 instances to the internet in general.  Of course, AWS supports this with
a Virtual Private Gateway and a Site-to-Site vpn.  They even give you instructions for setting
up the tunnel between a Microtik router and the AWS side.

There are, however, caveats.

1. As of May 2025, the provided instructions don't match the new RouterOS interface.  It isn't
too difficult to guess where the various parameters go.  If using a pre-shared key, you have to make
a new entry on the 'Identities' tab and tie that to the peer.

1. The instructions will tell you to attach a 'tunnel interface' to your WAN address.  This is just
wrong. Ignore that part.

1. If you're using BGP, the instructions leave out this important detail: you need to turn on 'Route
Propagation' in the Route Table associated with your VPC. (VPC Dashboard > Route Tables > Route Propagation)

