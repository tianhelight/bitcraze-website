---
layout: page-product
title: Loco Positioning system
permalink: /loco-pos-system/
page_id: product-loco-pos-system
---

{% buy_online https://store.bitcraze.io/collections/positioning/products/indoor-explorer-bundle %}

{% product_highlight
fa-location-arrow;
Position awarenes;
Add absolute position to your Crazyflie 2.0 using the Loco Positioning system.
%}

The Crazyflie 2.0 (as most other quadcopters and robots) has no real notion of
its position in space. The on board sensors (accelerometers and gyros) can be
used to give a rough idea of its movements but lacks the accuracy for long term
position awareness. The solution is to use an external system that can provide
information of the current position. Outside GPS can be used, but indoor the
options are limited, often complex, expensive or both. That is why we have
created the Loco Positioning system.

#### The system

The Loco Positioning system is a local positioning system that is used to find
the absolute 3D position of objects in space. It is in many ways similar to a
miniature GPS system.
The base of the system is a set of Anchors that are positioned in the room
(compare to the satellites in GPS), they are the reference. The other part of
the system is one or more Tags (compare to the GPS receiver) that are fixed to the
object(s) that are to be tracked. By sending short high frequency radio
messages between the Anchors and Tags, the system measures the distance from
each Anchor to the Tags and calculates the position of the Tags from that
information.
All information needed to calculate the position is available in the Tag which 
enables position estimation on board of the Crazyflie, as opposed to many other
positioning systems where the position is calculated in an external computer
and sent to the Crazyflie.
By adding knowledge of its position to a Crazyflie 2.0 it is capable of flying
autonomously without manual control. This opens up an array of exciting use
cases and applications.

#### The Loco Positioning Deck

The Loco Positioning Deck is a Crazyflie 2.0 expansion deck with the Loco
Positioning Tag functionality. Read more on the [Loco Positioning Deck page.](/loco-pos-deck/)

#### The Loco Positioning Node

The Loco Positioning Node is a multi functional node in a Loco Positioning system,
it can act either as an Anchor or Tag. As an Anchor it is part of the reference base for
the system while running in Tag mode it can be attached to an object to track,
for instance a robot. Read more on the [Loco Positioning Node page.](/loco-pos-node/)

#### Performance

The Loco Positioning system is based on the Decawave DWM1000 chip and has an
accuracy in the 10 cm range.

A theoretical minimum of 4 Anchors are required to
calculate the 3D position of a Tag, but a more realistic number is 6 to add
redundancy and accuracy.

The current implementation is using the 2-way ranging mode and supports positioning
of one Tag. The hardware supports other modes that can track multiple Tags (swarming)
but the software is still experimental.

The Loco Positioning system has mainly been designed for indoor use.

## Getting started with Loco positioning

We have created a easy to follow step-by-step guide for setting up the Loco positioning system that you will find [here](/getting-started-with-the-loco-positioning-system/). In the tutorial we use the [Indoor explorer bundle](https://store.bitcraze.io/collections/bundles/products/indoor-explorer-bundle) that you can buy directly from our [E-shop](https://store.bitcraze.io/). For more technical information about the Loco positioning system please visit our [wiki](https://wiki.bitcraze.io/doc:lps:index).

## Used by Lund University

At the [Centre for Mathematical Sciences](http://www.maths.lu.se/english) at [Lund University](https://www.lth.se/english)
PhD student Kenneth Bastone and professor Kalle Åström are currently using the
Crazyflie and the Bitcraze ultra-wide band based Loco Positioning system as part
of their research. We visited them and wrote a blog post about their work.

{% img Centre for Mathematical Sciences; medium; /images/portals/research/lps-research-loco-positioning-kalle-åström-768x512.jpg %}

To read the blog post go [here](https://www.bitcraze.io/2016/06/loco-positioning-in-lth-math-department/).
