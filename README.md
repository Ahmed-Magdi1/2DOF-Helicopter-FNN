# 2DOF Helicopter modeling using FNN

## Overview
This project models the nonlinear dynamics of a 2-DOF helicopter system using a Feedforward Neural Network (FNN). The model predicts the system's behavior based on input variables (voltage and motor currents) to output pitch and yaw angles.

## Colab Link
You can access the Google Colab notebook for this project: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1R4zDnM1aQhnxVBRMJRPPZ00QFcpnUQo8?usp=sharing)



## Data Used
The model is trained and validated using real data representing the helicopter's behavior:
- **Input Variables**:
  - `V`: Voltage applied to the motors (constant for both motors).
  - `I_pitch`: Current for the pitch motor.
  - `I_yaw`: Current for the yaw motor.
- **Output Variables**:
  - `pitch_angle (θ)`: The pitch angle of the helicopter.
  - `yaw_angle (ψ)`: The yaw angle of the helicopter.

### Data Format
The input and output data are stored in separate CSV files:
- [`inputs.csv`](inputs.csv): Contains columns `V`, `I_pitch`, `I_yaw`.
- [`outputs.csv`](outputs.csv): Contains columns `pitch_angle`, `yaw_angle`.
