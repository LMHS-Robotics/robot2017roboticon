# robot2017roboticon
Brandon's code, you owe me for this.
Robotbuilder videos: https://www.youtube.com/watch?v=UGSvE77Hpls&list=PLhwpRbR67J4aEIyWNE4p-IlIDJFm6kHLe



Editing ports:
Ports for all of the devices are found in the RobotMap.cpp file. Go there if you need to change ports of talons or solenoids. I explained how too in the file's comments.



Changing time of autonmous driving forward:
The autonomous is set to drive forward at half speed for 3 seconds. You can change the time in the AutonomousCommand.cpp file       under commands folder.
If you need to change the speed that can be done under the DriveTrain.cpp file under subsystems folder in the driveForward() function.



Compressor Turning On:
The compressor will only turn on if the robot is enabled in teleop or autonomous. For saftey reasons you cannot turn on the compressor when the robot is disabled (i.e, can't turn it on when robot boots). So for matches you need to enable it while queing so it can have full pressure when starting.




Joystick (xbox controller):
You may want to change which button does what. You can do this in the OI.cpp file. Simply change the number in the reset command for the button (i.e shifterButton.reset(new JoystickButton(stick.get(), 5)); you would change the 5 to the button number you desire)
Heres an image of the mapping for xbox controllers:
![alt text](http://i245.photobucket.com/albums/gg79/traycerb/Xbox360WirelessControllerImageX3.jpg)




Testing Talons:
Make sure you go into the roborio webpage and check to see everything is working and configured properly. Two can devices cannot have the same port so change ports as necessary so every device has a unique port. If you have talons not showing up it may mean multiple talons have the same port. Just change one of them (usually the one with port 0), refresh, then the other should appear.
