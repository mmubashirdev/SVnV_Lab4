# Autonomous Delivery Robot


## Extract Requirements

| Requirement_Id | Description | Priority |
|---|---|---|
| FR-01 | The robot shall remain in the idle state after being switched on until a delivery request is received. | High |
| FR-02 | The robot shall start navigating toward the specified destination when a valid delivery request is received. | High |
| FR-03 | The robot shall continuously monitor its surroundings for obstacles while navigating. | High |
| FR-04 | The robot shall temporarily stop normal navigation and enter obstacle-avoidance mode when an obstacle is detected. | High |
| FR-05 | The robot shall resume navigation toward the destination after successfully avoiding an obstacle. | High |
| FR-06 | The robot shall start the delivery process when it reaches the requested destination. | High |
| FR-07 | The robot shall return to the warehouse after successfully completing the package delivery. | High |
| FR-08 | The robot shall continuously monitor its battery level while navigating. | High |
| FR-09 | The robot shall stop the current delivery journey and return to the warehouse when the battery level becomes critically low. | High |
| FR-10 | The robot shall prevent the delivery process from starting unless a delivery request has been received, the destination has been reached, and the robot is not in obstacle-avoidance mode. | High |
