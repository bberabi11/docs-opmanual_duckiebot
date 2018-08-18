## Assembling the `DBV2` {#assembling_dbv2 status=beta}

Point of contact: Redesign Group

Once you have received the parts and soldered the necessary components, it is time to assemble them in a Duckiebot. Here, we provide the assembly instructions for the configuration `DBV2`.

<div class='requirements' markdown="1">

Requires: Duckiebot `DBV2` parts. The acquisition process is explained in [](#acquiring-parts-dbv2).

Requires: having soldered `DBV2` parts. The soldering process is explained in.

Requires: Having prepared the power cable. The preparation is explained in [](#power-cable-prep-c0). Note: Not necessary if you intend to build a `DBV2` configuration.

Requires: Time: about 40 minutes.

Results: An assembled Duckiebot in configuration `DBV2`.

</div>

This section is comprised of 8 parts. Each part buils upon some of the previous parts, so make sure to follow them in the following order.

- [Part I: Introduction](#all-pieces)
- [Part II: DC-Motor and Driving Mechanism](#howto-mount-dc)
- [Part III: Steering Mechanism](#howto-mount-steering)
- [Part IV: Servo](#howto-mount-servo)
- [Part V: Battery](#howto-mount-battery-hmb)
- [Part VI: Upper Plate](#howto-mount-deck)
- [Part VII: Raspberry Pi 3 B+ and MC-Board](#howto-mount-rpi-mc)
- [Part VIII Motors and LEDs connections](#howto-connections)


### Introduction {#all-pieces}

Open the _Tamiya 70112 Buggy Car Chassis_ and take out the components shown in [](#fig:parts_buggy). We will only need these parts out of the set.

<figure id="fig:parts_buggy" figure-caption="Relevant Components in Buggy Set">
     <img src="DSC_0202.jpg" style='width:30em'/>
</figure>


[](#fig:all_parts) shows all parts and components needed to assemble the `DBV2`.

<figure id="fig:all_parts" figure-caption="Components in Duckiebot package.">
     <img src="DSC_0200.jpg" style='width: 30em'/>
</figure>

### DC-Motor and Driving Mechanism {#howto-mount-dc}

In a first step, the dc-motor has to be inserted into the driving mechanism. Do not be afraid to press. Once assembled, this component should look like . x The parts necessary for this are depcited in [](#fig:dc_assmbl).


<figure id="fig:dc_assmbl" figure-caption="DC Motor">
     <img src="DSC_0203.jpg" style='width: 30em'/>
</figure>



Now, simply use the two nylon screws and both hex nuts to tighten the driving mechanism to the lower plate as shown in
[](#fig:dc_wheels).


<figure id="fig:dc_wheels" figure-caption="Assembled dc-motor">
     <img src="DSC_0204.jpg" style='width: 30em'/>
</figure>


[](#fig:lateral) will make sure you connect both parts through the correct holes.

<figure id="fig:lateral" figure-caption="Assembled dc-motor">
     <img src="DSC_0205.jpg" style='width: 30em'/>
</figure>


The next step is to connect the two bigger wheels to the driving mechanism. Use the _name?_ ([](#fig:wheels_1)) and proceed as explained below:

<figure id="fig:wheels_1" figure-caption="Driving Mechanism: Parts">
     <img src="DSC_0207.jpg" style='width: 30em'/>
</figure>



Insert the _name?_ first, then do the same with the wheels
([](#fig:dc_wheels_half)).

<figure id="fig:dc_wheels_half" figure-caption="Components in Duckiebot package.">
     <img src="DSC_0208.jpg" style='width: 30em'/>
</figure>


The end result of this part should look like [](#fig:drive_assmbl).



<figure id="fig:drive_assmbl" figure-caption="Assembled Rear Part">
     <img src="DSC_0209.jpg" style='width: 30em'/>
</figure>

### Steering Mechanism {#howto-mount-steering}

Once the driving mechanism is done, we will now focus on the steering mechanism. All the pieces needed to do this are shown in [](#fig:front_all).

<figure id="fig:front_all" figure-caption="Steering Mechanism: Parts 1">
     <img src="DSC_0210.jpg" style='width: 30em'/>
</figure>

First, connect the _name?_ with the plexiglas part with the screws and secure this with the hexnuts.

Continue by glueing the rotating part to the plate. Make sure you insert it into the middle hole.

The images below will help you visualize this procedure:

<figure id="fig:front_all_2" figure-caption="Steering Mechanism: Step 1">
     <img src="DSC_0211.jpg" style='width: 20em'/>

</figure>
<figure id="fig:front_all_3" figure-caption="Steering Mechanism: Step 2">
     <img src="DSC_0213.jpg" style='width: 20em'/>
</figure>

<figure id="fig:front_all_4" figure-caption="Steering Mechanism: Step 3">
     <img src="DSC_0215.jpg" style='width: 20em'/>
</figure>

Now, insert the long screws together with the two golden _name?_ into both wheels and connect them to the steering mechanism you just assembled:

<figure id="fig:front_wheels_1" figure-caption="Front Wheels: Step 1">
     <img src="DSC_0216.jpg" style='width: 20em'/>
</figure>

<figure id="fig:front_wheels_2" figure-caption="Front Wheels: Step 2">
     <img src="DSC_0217.jpg" style='width: 20em'/>
</figure>

<figure id="fig:front_wheels_3" figure-caption="Front Wheels: Step 3">
     <img src="DSC_0218.jpg" style='width: 20em'/>
</figure>

The end result of these two steps should look like [](#fig:steer)
<figure id="fig:steer" figure-caption="Steering mechanism: Step 3">
     <img src="DSC_0219.jpg" style='width: 30em'/>
</figure>  


### Servo {#howto-mount-servo}

To connect the steering mechanism to the lower plate, first install the servo. The necessary parts are shown in [](#fig:servo_parts).

<figure id="fig:servo_parts" figure-caption="Servo Installation: Parts">
     <img src="DSC_0220.jpg" style='width: 30em'/>
</figure>

Place the servo inside the biggest hole in the front part of the lower plate ([](#fig:servo_in)).

<figure id="fig:servo_in" figure-caption="Servo Installation: Step 1">
     <img src="DSC_0222.jpg" style='width: 30em'/>
</figure>

Tighten the servo to the lower plate using two screws and three hexnuts [](#fig:servo_installed).

> Note: The screw in the front needs an additinal hex nut on top so that the steering mechanism moves unhindered.

<figure id="fig:servo_installed" figure-caption="Servo Installation: Step 2">
     <img src="DSC_0223_1copia.jpg" style='width: 30em'/>
</figure>


> Do not worry about the picture showing the steering mechanism already connected to the plate. You will do so no, it only shows the connection with both nylon screws and three hex nuts.

Now, simply connect the steering mechanism to the lower plate by inserting the rotor into the servo motor. See the images below for clarification.

<figure id="fig:servo_insert_1" figure-caption="Servo Placement">
     <img src="DSC_0224.jpg" style='width: 30em'/>
</figure>

<figure id="fig:servo_insert_2" figure-caption="Servo Securement">
     <img src="DSC_0225.jpg" style='width: 30em'/>
</figure>

Tighten the connection with the small black screw included in the servo set ([](#fig:steering_plate)).

<figure id="fig:steering_plate" figure-caption="Servo Installation: Step 3">
     <img src="DSC_0227.jpg" style='width: 30em'/>
</figure>

Take 12 nylon standoffs, make four groups of three and screw them together as shown below:

<figure id="fig:standoffs_1" figure-caption="Standoffs">
     <img src="DSC_02271.jpg" style='width: 20em'/>
</figure>

<figure id="fig:standoffs_2" figure-caption="3xStandoffs">
     <img src="DSC_02272.jpg" style='width: 20em'/>
</figure>

<figure id="fig:standoffs_3" figure-caption="3x4 Standoffs">
     <img src="DSC_02273.jpg" style='width: 20em'/>
</figure>


Introduce them into the bottom plate as shown in [](#fig:standoffs_plate). They will hold the deck.  
Use the Nylon hex nuts to fix the standoffs to the plate.

_This figure needs to be replace by one without the mechanisms connected!_
<figure id="fig:standoffs_plate" figure-caption="Standoffs for bottom plate">
     <img src="DSC_0228.jpg" style='width: 30em'/>
</figure>  

### Battery {#howto-mount-battery-hmb}

> Note: This is optional. It is strongly advised, though, since it will make sure the battery stays in its place.

As you may have appreciated, the images shown above depict the lower plate with two velcro stripes sticked to it.

Cut two equally long stripes from the other velcro roll and atach them to the battery.

This way, you make sure it will stay in place.

### Upper Plate {#howto-mount-deck}

Insert four standoffs, two nylon screws and connect the camera to the upper plate with the aid oftwo scres and two hex nuts.
[](#fig:deck_1) shows the exact places all screws and standoffs go in to.

<figure id="fig:deck_1" figure-caption="Upper PLate Preparation: Parts">
     <img src="DSC_0230.jpg" style='width: 30em'/>
</figure>

This procedure is illustrated below:


Proceed with the connection of the upper and lower deck:

Tighten the four screws with the standoffs from the lower plate. Make sure everything is tight.


### Raspberry Pi 3 B+ and Microcontroller Board {#howto-mount-rpi-mc}

Place the Raspberry Pi on top of the four standoffs and secure it with four additional standoffs ([](#fig:rpi_pie))

<figure id="fig:rpi_pie" figure-caption="Raspberry Pi">
     <img src="DSC_0231.jpg" style='width: 30em'/>
</figure>

Now, insert the Microcontroller Board into the Raspberry Pi through the stacking headers as in [](#fig:standoffs_deck).

<figure id="fig:standoffs_deck" figure-caption="Micrcontroller Board">
     <img src="DSC_0232.jpg" style='width: 30em'/>
</figure>


Place the Raspbery Pi's hole on top of the standoffs and fix these components with four additional standoffs.  
Then, insert the microcontrolles board into the Raspberry Pie with the stacking headers.  
The installation is illustrated below.

### Motors, Battery and LEDs connections {#howto-connections}

It remains to connect both motors to Microcontroller Board and to connect both boards to the battery.

First, connect the women to women jumper wires of the servo motor and the male to male jumper wires from the dc motor to the Microcontroller as shown in [](#fig:servo_mc).

<figure id="fig:servo_mc" figure-caption="Servo and DC to Microcontroller">
     <img src="DSC_0233.jpg" style='width: 30em'/>
</figure>

Insert the battery in between the two plates. Preferably, make sure the battery outputs are on the same side as the Microcontroller inputs ([](#fig:battery_bot)).

<figure id="fig:battery_bot" figure-caption="Battery">
     <img src="DSC_0237.jpg" style='width: 30em'/>
</figure>


Take the duckiebot and the bumpers holding the LEDs. Simply insert these bumpers into the upper plate using the holes made for this purpose. The duckiebot should look like [](#fig:bot_leds)

> Note: The bumper holding three LEDs goes in the front.

<figure id="fig:bot_leds" figure-caption="LEDs">
     <img src="DSC_0240.jpg" style='width: 30em'/>
</figure>

Lastly, connect the women to women jumper wire from the LEDs to the Microcontroller. [](#fig:leds_wire) shows the exact pin connection.

<figure id="fig:leds_wire" figure-caption="Servo and DC to Microcontroller">
     <img src="DSC_0241.jpg" style='width: 30em'/>
</figure>


Connect the Raspberry Pi and the Microcontroller Board to the Battery and you are ready to enjoy your duckiebot!
