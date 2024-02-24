# LineFollower V5.0

<table>
  <tr>
    <td>

## Description:
This is an robot made to follow a black line from start to finish for various competitions.

It uses:
- ATmega328p-AU as an microcontroller(used in arduino uno);
- 16 or 20Mhz crystal resonator;
- [TB6612FNG](https://github.com/Tonikiller10000/MotorDriver_1) DC motor driver;
- [ITR8307-TR8](https://github.com/Tonikiller10000/ITR8307-TR8_SensorBar) sensor bar;
- LI-PO battery
- 2x DC motors with low torque high speed gear box
- robot suport (Wood, 3d printed or any low weight matherial)
    </td>
    <td><img src="https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/w4.jpg" height = 400 width= 300 ></td>
  </tr>
</table>

<table>
  <tr>LineFollower V5.0</tr>
  <tr>
    <td><img src="https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/z3.png"></td>
    <td><img src="https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/z1.png"></td>
    <td><img src="https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/z2.png"></td>
  </tr>
</table>
<table>
  <tr>LineFollower V4.0(old design)</tr>
  <tr>
    <td><img src="https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/zz.jpg" height = 250 width= 250 ></td>
    <td><img src="https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/v41.png" height = 220 width= 250 ></td>
    <td><img src="https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/sch4.png" height = 250 width= 250 ></td>
  </tr>
</table>

### Programming:
[Programming of the robot](https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/w6.jpg): is done via UART protocoll with an [FTDI](https://github.com/Tonikiller10000/CH340G-FTDI-PROGRAMER) programming board. The code for the LineFollower is not ready. It uses the PID algorithm, and further documentation about this algorithm and the  source code for the robot will be posted this year.
 
### Design and mentions
[Robot support design considerations](https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/w3.png):
- to reach lower inertia, the components and the most of the mass of the robot should be placed on it\`s back;
- to reach a longer allowed response time from the sensor line detection to the mottor speed change it should be builted longer;
- to reach better torque on the wheels, it should be wider. 

> [!TIP]
> for mounting the motors use industrial motor holders, or use an better printing tehnique[(don/`t print it horisontalli)](https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/w1.jpg).

The next version will heve all in one board the driver and the controller, and the board will be the actual support.
Another further design will have a turbine for faster speeds.


## Links: 
- ATmega328p-AU (microcontroller): 
- LM78L05 (5V voltage regulator):
- Proof of work: https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/w2.mp4



