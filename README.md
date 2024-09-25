# Automated-Sentry-

Using Fusion 360 I designed the main firing compartment for the turret. I used flywheels from a nerf blaster to propell the foam bullets forward.
I used a 5V blower fan to push the bullets into the flywheels where a custom designed pipe had to be created in fusion 360. A small 5V mini
servo is also installed into into the firing component, this is to stop the flow on bullets from entering the firing chamber and to prevent
further blocks.

The ball are stored inside a hopper above the main chasis where can be refilled using a screwable lid. A custom made wheel is attached to a
coupler and then atttached to a high tourque dc motor. When the motor turns it will push balls into the firing chamber if the mini servo 
is retrached. The enclosure is made of a plastic so you can see the amount of bullets remaining in the hooper.

installed on the main chaisis the the camera holder, this holds the camera which is necessary for object detection algorithms, also inside
the camera holder is a rgb led that has been soldered to a pcboard with appropriate resistors, This is the show the differnet stages of the
robot (shoot, searching, loading)

the main chasis is held up by 2 legs, one leg has a 25kg servo motor attached to the main chasis to rotate up and down and the other leg has 
a bearing to ensure smooth movement when moving the head up and down.

The two legs are screwed into a custom plate, so it can swivel left and right on a servo. steel ball bearings are popped in the underside of the plate
so that it can move horizontally freely.

Inside the base house the electronics. 7V is obtained from the power supply which is used to power the 2 high tourque servo motors and the flywheel motors.
a flyback diode is placed across the flywheels to prevent flyback voltage. Two bypass capacitors are used to reduce noise ensuring smooth operation.
Using a diode we can decrease the voltage to 6.3V so we can power the mini servo. The flywheels and and high tourque motor is connected via a relay 
so it can be triggered by the arduino. The arduino can be fitted into a seperate striboard where ground are connected and all the inputs all also 
connected. Two switches are also installed, one is a power switch can that break power to the circuit and the other acts as a pull 
