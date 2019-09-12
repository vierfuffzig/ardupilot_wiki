.. _safety-notes:


=======================
ArduPlane safety notes:
=======================


.. note::
    While your autopilot is a trustworthy assistant, you are the responsible pilot in charge. Situational awareness is mandatory.
    While an autopilot's stabilization can help to improve your flying skills, being ready to quickly take over manual control at 
    any time might be the only chance to save your plane in case of unexpected situations. Check and know your airframe's basic 
    flight behaviour in manual modes, know how to quickly take over full manual control. Make sure you don't meet unexpected or 
    untested behaviour when switching to manual flight mode. 
    

.. warning::
    While a flight controller might apparantly allow to handle an airplane without fundamental flying skills, 
    there's basic requirements to meet for safely handling your airframe.


ArduPilot provides fully autonomous flight features with its defaults aiming at maximum safety on a wide variety of airframes.
As stall situations are a common cause for crashes, the code provides various features to prevent unfortunate flight 
conditions that might lead to a stall and crash. These measures are mostly based on **keeping up the airframe's airspeed**
as well as **keeping bank and pitch angles within reasonable limits**.


.. tip::
    See :ref:`stall prevention <stall-prevention>` for further detail.

.. note::
    The topic of saftey is fundamental in aviation and should be foremost on your mind. Choose your airframe's design, weight, size, 
    as well as your launch site and flightpath responsibly.

Mind that while stall prevention features can help to *avoid* stall situations, there's only limited chance to *recover* from a stall 
once it has actually happened, as long as the autpilot's stabilization is active. The stabilization routines will likely aggravate 
the stall situation by trying to counteract the airframe's increasing bank or pitch angle. Furthermore, there's design- and 
setup-specific features that determine how your plane behaves in case of a stall. Static margin and wing load might eventually differ 
on a single airplane depending on respective payload mass and position. 
While a light airframe with sufficient longitudinal stability and a favourable wing design might recover quickly from a stall as 
soon as it has gained enough airspeed again, an airframe with a small stability margin tuned for maximum performance and a 
compareably high wing load might stall into a violent spin situation that can only be recovered from in manual control mode, taking 
the required measures quickly and decisively. A sufficient altitude might increase the chance to recover, while at low altitudes there 
will hardly be enough time for reaction until the airframe hits the ground. An accelerated dive from an altitude of 50 m will likely 
be followed by ground impact within less than 2 seconds.

.. note::
    Testing your airframe's stall behaviour in safe altitude can help to save your plane in a stall situation. 
    Knowing your airframe's capabilities and required minimum airspeed at various attitudes helps to safely set your 
    attitude controller's limits, allowing safe and reliable performance in automated modes. 
    

.. warning::
    It is not recommended to have your airframe fly autonomous missions without having thoroughly tested its performance and 
    limitations within safe control range.


**To avoid a stall situation it is recommended to:**
=====================================================

1.: know your airframes limitations.

2.: setup your flightcontroller to respect these limitations with sufficient safety margin.

3.: avoid critical flight attitudes in automated flight modes.



**To recover from a stall situation it is mandatory to:**
=========================================================

1.: be able to safely fly your airframe in manual flight mode.

2.: know how to reliably identify a stall situation and know how to recover.

3.: be able to take over manual control at any time.

4.: fly at safe altitude.
