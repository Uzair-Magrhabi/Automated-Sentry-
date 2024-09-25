Automated Sentry System
Using Fusion 360, I designed the primary firing mechanism for the turret. The propulsion system utilises flywheels, adapted from a Nerf blaster, to launch foam projectiles. A 5V blower fan is employed to feed the projectiles into the flywheels, guided by a custom-designed pipe, also created in Fusion 360. To manage projectile flow and prevent blockages, a 5V mini servo is integrated into the firing component, controlling the entry of rounds into the chamber.

The projectiles are stored in a hopper positioned above the main chassis, which can be easily refilled via a screwable lid. A custom-built wheel, attached to a coupler and powered by a high-torque DC motor, pushes the projectiles into the firing chamber when the mini servo is retracted. The hopper enclosure is transparent, allowing visual monitoring of the remaining ammunition.

Mounted on the main chassis is a camera holder, crucial for running object detection algorithms. The holder also contains an RGB LED, soldered to a PCB with the appropriate resistors, which visually indicates the system's operational states (shooting, searching, loading).

The chassis is supported by two legs: one leg incorporates a 25kg servo motor for vertical rotation, while the other includes a bearing to ensure smooth motion when adjusting the turret's elevation. These legs are fixed to a custom-designed base plate, which allows for horizontal rotation via a servo. Steel ball bearings are integrated beneath the plate to facilitate smooth, free movement.

The base houses the electronics, drawing 7V from the power supply to operate the two high-torque servo motors and the flywheel motors. A flyback diode is installed across the flywheels to prevent back-voltage, while two bypass capacitors are used to minimise electrical noise, ensuring stable operation. A diode reduces the voltage to 6.3V for powering the mini servo. Both the flywheels and high-torque motor are controlled through a relay, which can be triggered by the Arduino.

The Arduino is mounted on a separate stripboard, where all grounds and input connections are organised. The system features two switches: one is a power switch that cuts the circuit’s power, and the other is an SPDT switch connected to the A4 pin on the Arduino, allowing the signal to either pull up to 5V or pull down to 0V depending on the switch position.

****
