[image1]: ./images/motor_controller.jpg

# Annex 03 : Car Chassis

For this project you need to purchase a four-wheel car chassis with rear wheel propulsion and front wheel steering mechanism.

Traditional four-wheel car chassis that you can find in the internet have a four-motor mechanism and steering is achieved by activating the two motors on either side of the car.

A car chassis with a front wheel steering mechanism allows you to steer the two front wheels like in a real car. By learning how t o use this car chassis you will be able to:

1. use all techniques that you will learn or have already learned in the CarND courses;
2. familiarize yourself with the mechanisms and issues that correspond to real-world problems.

The wheel system is well designed. There are two bearings on either side of the wheel that make the system very efficient and resistance free.

The motor that is provided with the kit is a JGA25-370. The nice thing is that the motor is connected through a gear reduction mechanism that is extremely simple to mount. the motor and the gears are made of metal and they are very resistant. The issue I found with this car chassis is that it is a bit loud when running at full speed.

The steering servo is attached to the front of the chassis through two L-shaped metal supports. The servo drives the steering angle of the front wheels through two adjustable bars, one of which connects both front wheels and the other connect to one of the two wheels.


## 01. The L298N Motor Controller

The L298N motor controller is a commonly used motor controller, also called H-bridge motor controller. The below image shows how a typical L298N motor controller looks like:

![alt text][image1]

The blue connectors are used to connect the external battery and the motor, whereas the black pins are used to connect the Arduino.

## 02. Arduino versus Raspberry Pi

Please notice that the H-bridge could have also been connected to a Raspberry Pi. The drawbacks of using the Raspberry Pi is that you only have one so-called PWM pin. A PWM pin is a pin that allows you to define output values in a certain range and not only output values of type 0 and 1. If a motor needs to be controlled with discrete values between full power and no power you need a PWM output. The other issue is that if used without external hardware you might experience jittering of the servo.

An Arduino on the other hand has more than one PWM and is extremely stable when controlling the L298N.

## 03. L298N Motor Controller assembly


## 04. L298N Motor Controller Arduino code

What things you need to install the software and how to install them

```
Give examples
```

#### Understanding the code

The **void setup()** function is run first with its content between brackets. The **Serial.begin(9600)** sets up the speed of the serial port to 9600 baud. The baud setting in the serial monitor window must match this value so that the Arduino and serial monitor window are communicating at the same speed.

The **void loop()** function is run second with all its content between brackets.
The **Serial.println("Hello, world!")** sends the text *Hello World!* to the serial / USB port for display in the serial monitor window.

## 05. Purchases and Downloads
The Arduino can be purchased from the following link:
[Purchase an Arduino here](https://store.arduino.cc/)

## Author

**Massimo Passamonti**: [email me](me@massimoslab.com)

## License

This project and its source code are licensed under the MIT License. [See MIT License](https://github.com/github/choosealicense.com/blob/gh-pages/LICENSE.md) file for more details.
