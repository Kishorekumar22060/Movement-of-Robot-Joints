# Ex-Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```python
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
  pos=[[1,30],[2,40],[3,90]]
  robot = getRobot()
  robot.driveJoints(0,0,0,0,0,0)
  delay(5)
  for i in pos:
    robot.Controller.moveJoint(i[0],i[1])
    delay(5)


```
## Output
### 1. Generic Articulated Robot
![WhatsApp Image 2023-10-31 at 10 01 11 AM-4](https://github.com/Kishorekumar22060/Movement-of-Robot-Joints/assets/141472136/568632b9-1d2c-4820-b625-37982359579c)


### 2. robot.driveJoints(0,0,0,0,0,0)
![1](https://github.com/Kishorekumar22060/Movement-of-Robot-Joints/assets/141472136/1b03d002-5ad1-4348-885c-3b34160d9255)


### 3. Movement of Joint1
![11](https://github.com/Kishorekumar22060/Movement-of-Robot-Joints/assets/141472136/f38a3bee-666e-4407-bcfc-2fe7f996d45c)


### 3. Movement of Joint2
![2](https://github.com/Kishorekumar22060/Movement-of-Robot-Joints/assets/141472136/20873521-bc15-470c-afab-53073b4e5341)


### 3. Movement of Joint3
![-3](https://github.com/Kishorekumar22060/Movement-of-Robot-Joints/assets/141472136/dcc7620e-364a-4cc0-9559-9cb70ebe75fc)


## Result 
Thus the different robots joints are moved with the help of python list.


