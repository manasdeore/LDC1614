# LDC16xx_lib

## Description

This is a library intended to simplify use of TI LDC16xx family sensors with I2C interface using Arduino.

## Installation

To install the library copy the .cpp and .h sourcefiles into your arduino library directory into a LDC16xx_lib folder (e.g. "C:\Users\your_user\Ardunio\libraries\LDC16xx_lib"). 

## Connection

Connection of TI LDC16xx evaluation board to Arduino MEGA. 

>**Note:**
>
> For other Arduino boards connection connection might be different: e.g. some boards have two I2C interfaces (SDA and SCL, or SDA1 and SCL1). For proper wiring consult https://www.arduino.cc/en/reference/wire. In your code you may programatically select use interface:
> ***
>		// create a new LDC sensor object, initialize I2C interface, clock of 100kHz or 400kHz is allowed
>		// you can select Wire or Wire1 interface if available on your board
>		ldc = new LDC16xx(Wire, 400000);
	
![alt text](https://bitbucket.org/itiadasm/ldc16xx_lib-arduino/raw/master/docs/schematic.png)

## Usage and examples

You can use example.ino as a template for your own code.