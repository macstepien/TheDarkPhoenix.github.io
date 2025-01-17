---
layout: post
title: Tank
permalink: /projects/tank
excerpt: |
  3D printed remotely controlled inspection robot
  <center><img width="600" src="/pics/12_tank/front_compressed.jpg"></center>
  <br>
date: 2019-03-27
order_number: 6
---
{% include button.html text="Github repository" icon="github" link="https://github.com/macstepien/Tank" color="#0366d6" %}

Remotely controlled inspection robot based on Raspberry Pi Zero.

{% include figure.html image="/pics/12_tank/front.jpg" width="600" height="800" %}

The robot can be teleoperated using a web browser, it works quite well in rough terrain:

{% include video.html id="aftyQMt_rrg" title="Tank demo" %}

Construction started with PCB:
{% include figure.html image="/pics/12_tank/pierwotna.jpg" width="600" height="800" caption="PCB with connected components"%}

The PCB was supposed to control the following components:
- 2 motors with encoders
- 3 servos
- SPI communication with Raspberry
- battery voltage measurements
- 2 LEDs (indicating low battery voltage and "power on")

{% include figure.html image="/pics/12_tank/testowanie.jpg" width="600" height="800" caption="Prototyping PCB"%}

As a power source I used a LiPol battery that was connected to 2 voltage converters: one for the microcontroller and one for servos. 

{% include figure.html image="/pics/12_tank/plytkawobudowie.jpg" width="600" height="800" %}

Parts of the construction were 3D printed using 
[https://www.thingiverse.com/thing:652851](https://www.thingiverse.com/thing:652851 "Construction")

{% include figure.html image="/pics/12_tank/plytka.jpg" width="600" height="800" caption="PCB"%}

The robot was controlled through a web browser, I used [https://hackaday.io/project/25092-zerobot-raspberry-pi-zero-fpv-robot/log/97988-the-new-zerobot-pro](https://hackaday.io/project/25092-zerobot-raspberry-pi-zero-fpv-robot/log/97988-the-new-zerobot-pro "Code"), modified to work with my SPI communication.
