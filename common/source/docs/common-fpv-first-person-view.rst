.. _common-fpv-first-person-view:

=======================
First Person View (FPV)
=======================

*First Person View* provides you with a true pilot's eye view while
flying by placing a video camera and transmitter on your vehicle paired
with a receiver and either an LCD or goggles on the ground.  An optional
OSD (On Screen Display) helps maintain orientation by providing aircraft
instrument overlay on your FPV monitor.

.. image:: ../../../images/fpv_titleImage.jpg
    :target: ../_images/fpv_titleImage.jpg

Recommended parts
=================

To set up an FPV system on your vehicle you will need to add a video transmission system, including a flight camera and a video transmitter on your vehicle, as well as a video receiver and a display device on ground. 
Ardupilot supports a variety of :ref:`flight controllers <common-autopilots>`, some of which are equipped with an onboard video overlay chipset, allowing to overlay flight data onto your flight camera's video, as well as an onboard power module that provides battery monitoring without additional periphereals required. While it is convenient to use an aio-type flightcontroller for FPV purposes, alternatively a standalone MinimOSD-type board can be added to any existent flightcontroller without an onboard video chipset.
The parts recommended for a typical FPV setup are:

-  A CCD- or CMOS-type FPV flight camera with wide dynamic range (WDR) to provide good video quality under varying lighting conditions.
-  A pair of video transmitter and receiver. Mind your country's legal restrictions on HF frequencies and transmitted power. A typical 5.8Ghz video transmitter/receiver pair usually is a good place to start from.
-  An :ref:`onscreen display <common-osd-boards-on-screen-display>`. If you're not using ArduPilot onboard OSD on an aio-type flight controller, it is recommended to add a standalone board like `MinimOSD <http://store.jdrones.com/jD_MiniOSD_V12_p/jdminiosd12.htm>`__
   for On Screen Display of aircraft data.
-  A battery to power the video receiver and display device in your ground station.

There are two basic options to display your flight cam's video on the ground. One is a monitor like the `Black Pearl <http://www.amazon.com/FlySight-Black-Pearl-Diversity-Integrated/dp/B00KR69WHY>`__, the other is to use dedicated FPV video goggles. While using goggles provides a more immersive flight experience, it may be prefereable to use a monitor in some cases. Mind that there are FPV-specific video goggles and monitors that come with builtin video receiver modules or optional module bays to facilitate your ground setup.

**Goggle options:**

-  `Fat Shark <http://www.fatshark.com/default.html>`__ has a wide range
   of goggles including the "Attitude" and "Dominator" that have been
   proven to work well. Most Fatshark goggles have options for video receiver modules. 
-  Low cost 320x240 resolution goggles (`example video <https://www.youtube.com/watch?v=tG-4JNpE2fc>`__) are not
   recommended because the higher resolution 640x480 (`example video <https://www.youtube.com/watch?v=ywqacXyjcNw>`__) or SVGA
   goggles provide a much better flying experience.

In addition you may wish to set-up a separate :ref:`camera gimbal <common-cameras-and-gimbals>`\ (perhaps with Go-Pro
attached) to record the flight in HD.

Connection diagram
==================

Here is a wiring diagram `created by IVC <http://beta.ivc.no/wiki/index.php/TBS_Discovery_graphic>`__ for a
TBS Discovery Quadcopter that includes an APM2 and MinimOSD:

.. image:: ../../../images/tbs_discovery_install_APM2.6withminimosdtbscore.jpg
    :target: ../_images/tbs_discovery_install_APM2.6withminimosdtbscore.jpg

FPV equipment on the vehicle requires aditional attention regarding clean power sources and separation of HF-critical components
like GPS and RC receiver to reduce the chance of interferences limiting your transmission ranges and video quality.

OSD setup
==========

A guide to ArduPilot's onboard OSD :ref:`can be found here <common-osd-overview>`.

The MinimOSD set-up guide :ref:`can be found here <common-minim-osd-quick-installation-guide>`.

User Videos / Blogs
===================

Richard Evan's FPV flight footage (recorded from the ground station) of
his Copter based quadcopter including MinimOSD

..  youtube:: KQOQYcf4Dbc
    :width: 100%

Stefan Cenkov's FPV flight footage (recoded from the ground station) of
his Plane running on VrBrain including MinimOSD.

..  youtube:: LxjtUl8Fw6o
    :width: 100%

Robert Mcintosh's in `Lone Pine California <https://diydrones.com/profiles/blogs/the-best-place-to-fly>`__
FPV Flight with HD video footage from GoPro camera

https://vimeo.com/70365435

Euan Ramsey's APM2 powered `TBS Discovery <https://diydrones.com/profiles/blogs/tbs-disco-apm-mounting-suggestion>`__. 
Note the TBS frame spreads the 2 front arms apart so the blades don't
interfere with the FPV and allow the camera to easily be mounted in
front

Safety Warnings Relating Specifically to FPV Flight
===================================================

-  Because of the limited field-of-view of the FPV camera you may not be
   able to easily see obstacles near the vehicle which may be why the
   `Academy of Model Aeronautics <https://www.modelaircraft.org/>`__
   requires that there be a second person acting as spotter for all FPV
   flights.
-  Be ready for loss of FPV video caused by flying beyond your FPV
   systems limits or interference from structures between you and the
   vehicle.
-  Know and recognise the FPV signal loss warning signs and be ready to
   shed the FPV equipment and retake line-of-sight control at all times.
-  FPV equipment can interfere with the vehicle's radio or GPS if placed
   too close
