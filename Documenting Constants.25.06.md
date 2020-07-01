###### Documenting Constants

| name             | Description                                                           | Type   | Value    |
|:----------------:|:---------------------------------------------------------------------:|:------:|:--------:|
| productName      | The name of the physical product                                      | string |«RoboBall»|
| versionNumber    | The SDK version number                                                | number | 1.6      |
| commStop         | Command code to send to the robot to stop it                          | number | 0x00     |
| commMoveForward  | Command code to send to the robot to move it forward                  | number | 0x01     |
| commMoveBackward | Command code to send to the robot to move itbackward                  | number | 0x02     |
| commTurnLeft     | Command code to send to the robot to turn it to the left              | number | 0x03     |
| commTurnRight    | Command code to send to the robot to turn to the right                | number | 0x04     |
| errBadSignal     | Error code to Inform: the robot receives a bad signal from the device | number | 0xFF01   |
| errBadCommand    | Error code to Inform: the robot doesn't recognize the command         | number | 0xFF02   |
| errBatteryLow    | Error code to inform: the robot's batteries are low                   | number | 0xFF03   |