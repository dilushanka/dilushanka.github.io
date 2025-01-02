---
layout: post
title:  "Samsung A105f Mic ways and diagnose"
date: 01-01-2025
categories: [Repair]
tags: [Samsung A105F, Mic lines, mic diagnose, mic not work, samsung]
---

# Samsung A10 Mic repair

In this post, I will talk about how to diagnose a Samsung or any Android mobile with a mic that is not working using easy steps. In this case, I used the A105F mobile. First, study the case before disassembling the phone.

## symptems

First, open the recording app on your mobile phone and try recording. Here you can check whether the mic is working or not. Also, since this Samsung phone has two mics, test each mic separately. Make a normal call and talk normally, try putting it in hands-free mode. If you can hear your voice on the other side when the speaker is turned on, it can be concluded that the microphone on the sub-board is faulty.

## Diagnose

In my case the sub-board mic is faulty. So I disassembled it and got the board out. First, check the diode mode in the mic pads. (posttive and 2.8v line)
I checked those pads on the connecter pin (image below). I put my multimeter red probe into GND ( SMD mic Plate ) and measured the value in the black probe. First, check Main_mic_P Pin and get OL. After I check Main_Mic_bias_2P8 and get the diode value.
but it is an abnormal value without the main board. because this SMD mic has two different diode values in those pins. but I get OL. so I decide to change Mic. If you need to diagnose further away i Put details below.

![samsung a10f sub board mic ways](assets/img/posts/galaxy-a105F-audio-sub.png)

## FIX

I used my hot air gun to remove the SMD mic and used 200 C, 50 airflow. Don't use Heat more time. because it causes damage to The board.
 now get known good SMD mic and solder it to the board. don't use more flux.

## Test

now check the pads and you get different values. your job is done. and reassemble the phone.

## More Test

Remove the back plate turn on the mobile and make the call. Now measure the voltage on 2.8v so you can check the main board mic 2.8v and subboard 2.8v because those 2.8v lines are the same. For some reason, you don't get subboard 2.8v and you can decide the line is missing. You can wire jumper the main board mic 2.8v line to the board.

## Note
This mobile has a series capacitor before the PM IC so you cannot see the diode value in the mic positive line. This works on you connect the board to the main board and measure the diode value in the mic line.
![samsung a10f sub board mic ways](assets/img/posts/Mic%20line%20serise.png)

