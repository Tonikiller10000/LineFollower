# LineFollower V5.0

## Description:

<table>
  <tr>
    <td>
    This is an robot made to follow a black line from start to finish for various competitions. 
    
It uses:
- ATmega328p-AU as an microcontroller(used in arduino uno);
- 16 or 20Mhz crystal resonator;
- [TB6612FNG](https://github.com/Tonikiller10000/MotorDriver_1) DC motor driver;
- [ITR8307-TR8](https://github.com/Tonikiller10000/ITR8307-TR8_SensorBar) sensor bar;
- LI-PO battery (7.2V)
- 2x DC motors with low torque high speed gear box
- robot suport (Wood, 3d printed or any low weight matherial)
    </td>
    <td><img src="https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/w4.jpg" height = 400 width= 300 ></td>
  </tr>
</table>

 ## LineFollower V5.0
<table>
  <tr>
    <td><img src="https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/z3.png"  height = 220 width= 250 ></td>
    <td><img src="https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/z1.png"  height = 220 width= 250 ></td>
    <td><img src="https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/z2.png"  height = 220 width= 250 ></td>
  </tr>
</table>

 ## LineFollower V4.0(old design)
<table>
  <tr>
    <td><img src="https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/zz.jpg" height = 250 width= 250 ></td>
    <td><img src="https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/v41.png" height = 220 width= 250 ></td>
    <td><img src="https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/sch4.png" height = 250 width= 250 ></td>
  </tr>
</table>

### How it works:
The board is like a custom arduino UNO board powered from an 7.2V Li-Po battery trouth an 5V voltage regulator. The 8 analog pins are used as inputs from the sensor bar and 6 digital pins are used for the TB6612FNG motor driver witch is powered dirrectly from the battery to give more power to the motors. The reset pin has a 10K pullup resistor witch is pulled down by the reset button when it is pressed. The UART and ICSP pins wore pulled out to program the code and the bootloader of the IC.


### Programming:
[Programming of the robot](https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/w6.jpg): is done via UART protocoll with an [FTDI](https://github.com/Tonikiller10000/CH340G-FTDI-PROGRAMER) programming board. The code for the LineFollower is not ready. It uses the PID algorithm, and further documentation about this algorithm and the  source code for the robot will be posted this year.
 


### Start remote:


Robochalange remote:
[Start switch website](https://p1r.se/startmodule/)
[Start switch github](https://github.com/p1rse/robot-sumo-start-module/)
[IR Receiver Diode - TSOP38238](https://www.sparkfun.com/products/10266)
[schematic1](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgnkNo1QEsxSPMNj7rN0opPGzlpkEMgxas9PnXUh-xvVR3l7UK27BbSvRroJmsxzwf3StBiDH0k4m-aEXX_4qJKeG5T4bKsfCBbcjgoykJYrBEhg5JI-Mr95yexPMCzkTw7kaGDIzET8ME/s1600/1235.png)
[schematic2](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjLlN9CDAmP0rq2BlWM0Xdsypyy7NfGZpMYkufZPUAMmgCRdU-KhBC8AvPr7iOOQAwod2Hw66K_vuib1FNqDIHNemtnMvlSue2krN2hfp39g73NuTcx5fEXUF8i5MbJ3re-paKH2Z_Cgq0/s1600/1234.png)
[Q&A](https://robochallenge.ro/faq)
[MORE](https://destroyer3000.blogspot.com/2013/03/start-module-implement-yourself.html)






### How PID control work/`s

[Here](https://www.youtube.com/playlist?list=PLn8PRpmsu08pQBgjxYFXSsODEF3Jqmm-y) you can learn more about PID and under this you can see 
an analog linefollower project with and without PID:
- https://www.nutsvolts.com/magazine/article/the_pid_controller_part_1
- https://www.ecircuitcenter.com/Circuits/op_pid/op_pid.htm
- https://control.com/textbook/closed-loop-control/analog-electronic-pid-controllers/
- https://www.youtube.com/watch?v=4Y7zG48uHRo&list=PLOSOqCeZCHL0Qxb6YyrvGzjCg9FLfzHYJ

### ///////////////////////////////
- Small linefollower with op amp:https://www.youtube.com/watch?v=zZmvL0TkllI&list=WL&index=15&t=25s


### Design and mentions
[Robot support design considerations](https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/w3.png):
- to reach lower inertia, the components and the most of the mass of the robot should be placed on it\`s back;
- to reach a longer allowed response time from the sensor line detection to the mottor speed change it should be builted longer;
- to reach better torque on the wheels, it should be wider. 
- to mount the motors use molderd plastic motor holders, or be carefull when printing [it](https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/w1.jpg). 
- the case was made with autodesk fusion 360 at the 3d printer and with some M3 screws.

The next version will have the motor driver soldered on the board and motors screwed dirrectly to it as the suport. 
Another version will have a turbine for better torque and faster speeds.


## Links: 
- ATmega328p-AU (microcontroller): 
- LM78L05 (5V voltage regulator):
- Proof of work: https://github.com/Tonikiller10000/LineFollower/blob/main/LineFollower_Pictures/w2.mp4














