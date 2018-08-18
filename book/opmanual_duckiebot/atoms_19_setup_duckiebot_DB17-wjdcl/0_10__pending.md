## `DBV2` Potential Developments

Point of contact: Redesign Group

This section describes different aspects of the protoype of `DBV2` that can be further developed.

- [Servo Motor](#servo_motor_sm2)
- [Frequency Prescaler](#frequency_prescaler)
- [LED Connections](#led_connections)
- [Low-Pass Filter](#low_pass_filter)
- [Automatic Gear](#automatic_gear)


### Servo Motor {#servo_motor_sm2}

The servo motor currently used has a torque sufficiently high to steer the vehicle even at zero speed.

However, if more weight were to be added to the `DBV2`, and to make sure nothing unexpected occurs when turning the front wheels, a more powerful servo could be purchased and used.

### Frequency Prescaler {#frequency_prescaler}

To this moment, the Raspberry Pi still beliefs it is part of the old Duckiebot. The frequency at which the Raspberry Pi communicates with the Microcontroller that drives the servo and the dc motor can not be chosen freely: For the servo to work, a frequency has to be chosen that enables PWM signals being in the 'high' position from 1 ms to 2 ms.

A frequency too high makes this impossible. The lower the frequency, the more precisely the servo motor can be controlled. However, the lower the frequency, the longer the time from command to actual action.

Hence, the prescaler has to be selected in a way that guarantees both the servo to be sufficiently precise and the hole system to work with a low delay.

### LED Connections {#led_connections}

The current way in which the LEDs are part of the `DBV2`is the main aesthetic problem.

The LEDs are soldered together, which causes an unpleasant mess of cables.

Marcus Aaltonen has designed bumpers for the old Duckiebot that have the circuits to connect the LEDs integrated, making any additional cables unnecessary.

A great way to solve this aesthetic problem is to integrate such circuits into the bumpers used for `DBV2`.

### Low-Pass {#low_pass_filter}

The signal from the Microcontroller to the LEDs includes plenty of noise. Adding a Low-Pass filter to this connection will eliminate this problem. The integration of this filter into the PCB would make a pleasantly looking solution possible.

### Automatic Gear {#automatic_gear}

The `DBV2` includes the possibility of changing gears manually. Making the gear change automatic would make the `DBV2` even more car-like.
