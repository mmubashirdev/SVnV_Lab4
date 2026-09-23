# Transactions Table

| Transaction ID | From State | Event | To State | Requirement |
|---|---|---|---|---|
| TR-01 | IDLE | Delivery request is received | NAVIGATING | FR-01, FR-02 |
| TR-02 | NAVIGATING | Obstacle is detected | AVOIDING_OBSTACLE | FR-03, FR-04 |
| TR-03 | AVOIDING_OBSTACLE | Obstacle is successfully avoided | NAVIGATING | FR-05 |
| TR-04 | NAVIGATING | Destination is reached | DELIVERING | FR-06 |
| TR-05 | DELIVERING | Package is successfully delivered | RETURNING | FR-07 |
| TR-06 | NAVIGATING | Battery becomes critically low | RETURNING | FR-08, FR-09 |
| TR-07 | RETURNING | Robot reaches the warehouse | IDLE | FR-01 |
| TR-08 | IDLE | Delivery process is requested without a delivery request and destination reached | IDLE | FR-10 |
| TR-09 | AVOIDING_OBSTACLE | Delivery process is requested while handling an obstacle | AVOIDING_OBSTACLE | FR-10 |
