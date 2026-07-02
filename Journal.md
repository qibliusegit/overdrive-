
---
title: "Overdrive!!"
author: "Dhruv Ravinuthala"
description: "Basic distortion pedal"
created_at: "2026-07-01"
(Times are in Central Time)


---
# **July 2nd**

3:06 AM - tl;dr: I'm pretty new to KiCAD, so this was an experience. I finished up most of the circuit for the pedal and started working on power.

I installed KiCAD a while back for a Hackpad I was going to work on, though the bass I'm now working on took up too much planning time for me that. But thanks to Outpost's hardware requirements, I had an excuse to use it! (also I really wanted to make more stuff related to music).

After doing a good amount of research June 30th and July 1st, I found out that distortion and overdrive pedals aren't actually that complicated at all, since all they essentially do is clip the signal of the waves the guitar's strings make when vibrating. Because of this, you can make a pedal that doesn't need to be digital in the slightest.

Thanks to a good amount of documentation online, making the main circuit for the actual pedal wasn't very hard. I had a lot of material to cross-reference, as well as a good amount of content creators that have made videos on each step of building an overdrive pedal.
<img width="1223" height="716" alt="image" src="https://github.com/user-attachments/assets/ecc71270-4d74-4df7-a115-874442e37230" />

*fun fact: the original goal was to make a Boss Blues Driver (BD-2), but unfortunately that pedal emulates tubes, so it was a little out of my league.*

After this, I began work on power, and this was where a lot more issues started to arise, since I was working on this pretty much blind. I used whatever info I could find online on how power systems work in KiCAD and for guitar pedals, but thanks to not using a microcontroller and/or a breadboard, there was a severe lack of information in that department. I ended up *somewhat* getting the power system started, though I'm afraid it's nowhere near complete :(.

<img width="1223" height="716" alt="image" src="https://github.com/user-attachments/assets/1e7ca7da-9c2a-4c10-a0b0-b90ca3d9cd09" />

*i actually don't know if AC/DC named themselves after alternating and direct current. I wonder what Nikola Tesla would think if there was a rock band named after something he invented. Or if he would like heavy metal in general*

Time spent working: 1 hour 30 minutes


2:40 PM - tl;dr I made the circuit actually work like it's supposed to and look like it's supposed to.

Most of today was just working on whatever errors I had left, and making sure that everything was working properly. The first thing I did was mark things that didn't need connections so the electronic checker wouldn't show those as errors. After that, I seemed to be free of errors! However, that was far from the truth.

Thanks to a plethora of wonderful people on KiCAD's Discord Server, I was able to identify some other problems I had, the main one being that power wasn't properly being routed into my op amp. Rather than have power go immediately into my input jack like it was then, I actually needed power after the capacitor before my op amp. And speaking of my op amp? Yeah, I had to change which one I was using due to fanciness and practicality, though it didn't really alter the schematic much more than changing a couple numbers on the label.

After fixing that, I made a voltage divider, since the way the op amp works is by doubling the voltage of my signal. Also because of this, I switched my power in to 9 volts rather than 4. I originally had 4V because I thought I had to cut it in half myself, but nope! I build the thing that does it for me!
<img width="1223" height="716" alt="image" src="https://github.com/user-attachments/assets/58b6b781-28da-43fd-8bc2-c18fd633a07f" />

*So apparently the lead singer of AC/DC saw the letters on a plug for a sewing machine? This could be wrong, it's just something one of my friends told me. Would be really funny though.*

Time spent working: 1 hour 45 minutes




