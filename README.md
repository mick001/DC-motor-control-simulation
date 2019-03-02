## DC motor control simulation in Matlab and Simulink

A simulation of a control loop for a DC motor.

Two control strategies have been implemented through the use of a PI regulator:

1. Linear voltage control
2. PWM control

The files in this repository are the following:

- DC_motor.slx which is the Simulink model of the DC motor
- PWM.slx which is a simulink model for a PWM block (input=analogue voltage from 0 to 1 V, output=PWM signal to static switch)
- State space system: motor parameter, state space system and step response
- DC-motor-analogue-control.slx: Simulink model of a linear voltage control through a PI regulator
- DC-motor-pwm-control.slx: Simulink model of a PWM control through a PI regulator

The regulator was tuned with some overshoot using the tuning utility in Matlab.

### Control loop
![PWM control](https://user-images.githubusercontent.com/13961654/53666004-3df3cb00-3c6d-11e9-8f61-2fe56ec14dc8.png)
![Linear voltage control](https://user-images.githubusercontent.com/13961654/53666006-3f24f800-3c6d-11e9-87f5-8113fb4e0dcb.png)

### DC motor model implementation
![dc-motor](https://user-images.githubusercontent.com/13961654/53666767-4ea54080-3c6f-11e9-9af9-219a589f9025.png)

#### Speed variation [rad/s]
![speed-control-example](https://user-images.githubusercontent.com/13961654/53666772-52d15e00-3c6f-11e9-933a-781240180f96.png)
