[image1]: ./images/sdc_1.jpg
[image2]: ./images/sdc_10.jpg
[image3]: ./images/sdc_11.jpg

# Annex 03 : Car Chassis

For this project you need to purchase a four-wheel car chassis with rear wheel propulsion and front wheel steering mechanism.

Traditional four-wheel car chassis that you can find in the internet have a four-motor mechanism and steering is achieved by activating the two motors on either side of the car.

A car chassis with a front wheel steering mechanism allows you to steer the two front wheels like in a real car. By learning how t o use this car chassis you will be able to:

1. use all techniques that you will learn or have already learned in the CarND courses;
2. familiarize yourself with the mechanisms and issues that correspond to real-world problems.

The image below shows the car chassis as it is after assembly:

![alt text][image1]

The wheel system is well designed. There are two bearings on either side of the wheel that make the system very efficient and resistance free.

The motor that is provided with the kit is a JGA25-370. The nice thing is that the motor is connected through a gear reduction mechanism that is extremely simple to mount. the motor and the gears are made of metal and they are very resistant. The issue I found with this car chassis is that it is a bit loud when running at full speed.

The steering servo is attached to the front of the chassis through two L-shaped metal supports. The servo drives the steering angle of the front wheels through two adjustable bars, one of which connects both front wheels and the other connect to one of the two wheels.

## 01. Car chassis kit

The packaging of the car chassis contains mainly metal parts which ensures durability. The ratio quality vs prices is very good. Below is an image of the content of the cars chassis kit that you will receive.

![alt text][image2]

The actual chassis is also of very resistant metal, compared to many other car chassis that you can find online which are made of plastic:

![alt text][image3]

## 02. Car chassis assembly

Please notice that the H-bridge could have also been connected to a Raspberry Pi. The drawbacks of using the Raspberry Pi is that you only have one so-called PWM pin. A PWM pin is a pin that allows you to define output values in a certain range and not only output values of type 0 and 1. If a motor needs to be controlled with discrete values between full power and no power you need a PWM output. The other issue is that if used without external hardware you might experience jittering of the servo.

An Arduino on the other hand has more than one PWM and is extremely stable when controlling the L298N.


## 03. Purchases
The Arduino can be purchased from the following link:
[Purchase an Arduino here](https://store.arduino.cc/)

## Author

**Massimo Passamonti**: [email me](me@massimoslab.com)

## License

This project and its source code are licensed under the MIT License. [See MIT License](https://github.com/github/choosealicense.com/blob/gh-pages/LICENSE.md) file for more details.
