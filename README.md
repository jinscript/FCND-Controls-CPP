# The C++ Project Readme #

This is the readme for the C++ project.

## Body Rate Control

Implemented in `QuadControl::BodyRateControl(V3F pqrCmd, V3F pqr)`.

Formula:
![body_rate](formula/body_rate.png)

## Roll Pitch Control

Implemented  in `QuadControl::RollPitchControl(V3F accelCmd, Quaternion<float> attitude, float collThrustCmd)`.

Formula:
![altitude](formula/roll_pitch1.png)
![altitude](formula/roll_pitch2.png)

## Altitude Control

Implemented in `QuadControl::AltitudeControl(float posZCmd, float velZCmd, float posZ, float velZ, Quaternion<float> attitude, float accelZCmd, float dt)`.

Formula:
![altitude](formula/altitude1.png)
![altitude](formula/altitude2.png)
![altitude](formula/altitude3.png)

## Lateral Position Control

Implemented in `QuadControl::LateralPositionControl(V3F posCmd, V3F velCmd, V3F pos, V3F vel, V3F accelCmdFF)`.

Formula:
![lateral](formula/lateral.png)

## Yaw Control

Implemented in `QuadControl::YawControl(float yawCmd, float yaw)`.

Formula:
![yaw](formula/yaw.png)

## Motor Command Generation

Implemented in `QuadControl::GenerateMotorCommands(float collThrustCmd, V3F momentCmd)`.

Formula:
![motor_gen1](formula/motor_gen1.png)
![motor_gen2](formula/motor_gen2.png)
