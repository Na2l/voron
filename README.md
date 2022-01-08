# voron 2.4 350 mm
https://www.youtube.com/watch?v=3hocvaTHagI&ab_channel=NERO3D


<h2>Octopus pro board config</h2> 
https://docs.vorondesign.com/build/startup/
<p>
Here are the steps in the correct order:

<h2>1- Jumper settings</h2>
<li style="color:red" > Red: Remove Jumper</li>
<li  style="color:red" > Green: add Jumper</li>
</ul>
<img src='https://docs.vorondesign.com/build/electrical/images/v2-octopus-initial-preparation.png'>

<h2>2- Wire configuration</h2>
<h3>2a) V2 MOTOR POSITIONS</h3>
<img src='https://docs.vorondesign.com/build/startup/images/V2-motor-positions.png'>
<h3>2b) Wire configuration</h3>
<img src='https://docs.vorondesign.com/build/electrical/images/v2_octopus_wiring.png'>
<h2>3- printer.cfg<h2>
https://github.com/Na2l/voron/blob/main/printer.cfg
is configured and tested to be working with the settings mentioned in this README file.


<h3>To verify that each stepper motor is operating correctly, send the following commands in the terminal.</h3>

<b>Note</b>: Z motors will move UP first and then DOWN 3 times, one second apart.<br>
<b>Note</b>: looking at the front of the hotend, X Will move to the lef and then right 3 times, one second apart.<br>
<b>Note</b>: facing the fornt of the hotend, Y Will move forwards to you and then back 3 times, one second apart.<br>

<b>
 If the steppers do not move or make strange noises, check the wiring. Be sure to watch the Z motion to ensure the direction is correct. If the Z motor(s) do not move in the correct directions, invert the DIR pin on the printer configuration.
</b>

<ul><b>Commands</b>
<li>STEPPER_BUZZ STEPPER=stepper_x</li>
<li>STEPPER_BUZZ STEPPER=stepper_y</li>
<li>STEPPER_BUZZ STEPPER=stepper_z</li>
<li>STEPPER_BUZZ STEPPER=stepper_z1</li>
<li>STEPPER_BUZZ STEPPER=stepper_z2</li>
<li>STEPPER_BUZZ STEPPER=stepper_z3</li>
 </ul>

<h3>3- XY Homing Check</h3>
see here: https://docs.vorondesign.com/build/startup/#xy-homing-check
<p>
Wiring troubleshooting 
</p>
<img src='https://docs.vorondesign.com/build/startup/images/V2-motor-configuration-guide.png'>

https://docs.vorondesign.com/build/startup/
