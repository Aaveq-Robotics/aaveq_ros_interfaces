# Aaveq ROS 2 Interfaces

This package contains the ROS 2 interfaces for projects by Aaveq Robotics.

## Messages

### `ControlOutput.msg`

Control output from ArduPilot SITL simulation.

| Data          | Description                                       | Datetype      |
| ---           | ---                                               | ---           |
| `servo_pwm`   | Control output from ArduPilot's SITL simulation   | `uint16[]`    |


### `SimState.msg`

Simulation state feedback for ArduPilot SITL simulation. 

| Data          | Description                   | Datetype                  |
| ---           | ---                           | ---                       |
| `timestamp`   | Time stampt for simulation    | `uint64`                  |
| `gyro`        | Gyro data                     | `geometry_msgs/Vector3`   |
| `accel`       | Accelerometer data            | `geometry_msgs/Vector3`   |
| `position`    | Position data                 | `geometry_msgs/Vector3`   |
| `attitude`    | Attitude data                 | `geometry_msgs/Vector3`   |
| `velocity`    | Velocity data                 | `geometry_msgs/Vector3`   |

