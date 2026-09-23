# Lab Scenario: Autonomous Delivery Robot

## States


| State_Id | Statename | Description | Entry Condition | Exit Condition |
|---|---|---|---|---|
| ST-01 | IDLE | The robot is at the warehouse and waits for a delivery request. | Robot is switched on or returns to the warehouse. | A valid delivery request is received. |
| ST-02 | NAVIGATING | The robot moves toward the requested delivery destination. | A valid delivery request is received while the robot is IDLE, or an obstacle has been avoided. | Destination is reached, an obstacle is detected, or battery becomes critically low. |
| ST-03 | AVOIDING_OBSTACLE | The robot temporarily stops normal navigation and handles a detected obstacle. | An obstacle is detected while NAVIGATING. | The obstacle is successfully avoided. |
| ST-04 | DELIVERING | The robot delivers the package at the requested destination. | The robot reaches the destination while NAVIGATING. | Package is successfully delivered. |
| ST-05 | RETURNING | The robot travels back to the warehouse after delivery or due to critically low battery. | Package is delivered or battery becomes critically low during navigation. | The robot reaches the warehouse. |
