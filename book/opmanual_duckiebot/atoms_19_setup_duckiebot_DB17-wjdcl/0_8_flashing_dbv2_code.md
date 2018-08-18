## Flashing the Code to the Microcontroller Board (`DBV2`) {#flashing_the_code status=beta}

Point of contact: Redesign group

Once you have assembled the `DBV2`, it is time to flash the code to the Micrcontroller Board.

> Note: This is necessary since the code already on the Raspberry Pi is not adapted to drive a four-wheeler.

<div class='requirements' markdown="1">

Requires: An assembled `DBV2`. The procedure is documented in [](#assembling_dbv2).  

Requires: You have configured the Duckiebot. The procedure is documented in [](#setup-duckiebot).  

Requires: Approximately 2 minutes.  

Results: A functional `DBV2`.  

</div>

It is imperative that the Microcontroller Board is correctly connected to the Raspbeery Pi through the stacking header and that both boards are connected to the battery. Make sure the lights and connections on these boards coincide with the ones shown in [](#fig:boards_connections).

<figure id="fig:boards_connections" figure-caption="Raspbery Pi and Microcontroller Board">
     <img src="" style='width:30em'/>s
</figure>

In a first step, ssh into your duckiebot.  

Make sure you have downloaded the latest software version from Github:

    duckiebot $ sudo apt update
    duckiebot $ sudo apt dist-upgrade

Now, enter the following command:

    duckiebot $ cd duckietown/hardware/traffic-light/software_dbv2

To flash the code on the Microcontroller Board, enter the following commands:

    duckiebot $ make fuses
    duckiebot $ make clean
    duckiebot $ make

_Add expected terminal results_

### Test the motors

One way to test the proper working of the `DBV2` is to execute the RC remote control test.

> Note: If you want to perform the test, but you haven't gone through the setup described in [](#rc-control), do it now.

If you haven't already, ssh into your duckiebot.

Go into to duckietown directory:

    duckiebot $ cd ~/duckietown

Enter the following commands:

    duckiebot $ source environment.sh

    duckiebot $ roslaunch duckietown joystick.launch veh:=![robot name]

Test the car. Enjoy!

### Test the LEDs

If you haven't already, ssh into your duckiebot.

In order to test the proper functioning of the LEDs, execute the following commands:

    duckiebot $ cd ~/duckietown
    duckiebot $ source environment.sh
    duckiebot $ rosrun rgb_led blink test_all_1

Visually, you should expect the following pattern:

1. All light blink red, once;
2. All lights blink green, twice;
3. All lights blink blue, three times.
4. One configuration is held constant for some seconds.
5. Repeat at 1.

One additional test is to set the color and frequency of all lights:

    duckiebot $ cd ~/duckietown
    duckiebot $ source environment.sh
    duckiebot $ rosrun rgb_led blink <all>-<![color]>-<![frequency]>

![color]: blue, red or green.
![frequency]: 1.0, 2.0, etc.

> Note: Not all frequencies work.
