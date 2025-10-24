---
description: Journey to our first flight computer
---

# SNS 1

### What does a flight computer look like at the model scale?&#x20;

To build a computer we first need its brain, a CPU, in Our case it will be a microcontroller.\
**The microcontroller** acts as the brain by processing all the data received by various sensors on board.

Now with the brain in our hands, we can gather data and process it.

The first important sensor for model rocket Avionics is the IMU or the **inertial measurement unit.**\
It has a set of accelerometers and gyroscopes that determine the orientation and acceleration of our rocket.

The next thing we need is a **Barometric and Pressure Sensor** it gives us the current pressure and the altitude of our rocket (altitude is kind of the only thing we require for the first model rocket)

We can also add a **GPS sensor** onboard to precisely track our rocket.

The microcontroller also controls the **Active controls in the system** (like a TVC gimbal or actuating fins)

To regain our model safely we also require a recovery system and parachutes are used for recovery. **The parachute ejection system** is also controlled by the microcontroller.

**Power source.** We need a power source generally a battery to power all the sensors and the microcontroller.

Another useful thing could be **State Indicator(s).** State indicators help us ease through the flight preparation process. So that we don't have to go through all the reading if there's any problem &#x20;

The last thing we need is a **Data Recorder.**&#x20;

### What are all the different Sensors and Microcontrollers?

#### Microcontrollers

There are quite a few that we have tried

* Arduino UNO
* Arduino NANO
* Arduino Micro
* Raspberry pi
* ESP8266
* ESP32

**IMUs (Inertial Measurement Unit)**

There are two majorly used IMU units

* MPU6050
* Bosh BNO5

#### Barometric and Pressure sensors

Here we have too  many options but the most common ones used are:

* BMP280
* BMP380

#### GPS unit

we haven't done too much research into GPS units for now as we are not actively using them. But the one we are currently working with is the **NEO-6m GPS module**

#### Parachute ejection system

For the parachute ejection system, we simply use gunpowder to make a small explosion that blasts the parachute out.&#x20;

We use transistors as switches to ignite the gunpowder. Which I'll discuss in detail with the flight computer

#### Active Control systems

Active control systems use servo motors to actuate the fins or TVC mount which are controlled by the microcontroller (Servo motor SG90)

#### Power Source&#x20;

The Avionics system is generally powered by a battery.

LIPO batteries are the best way to go.&#x20;

Important things that should be kept in mind while selecting a battery

* Voltage and mAh( milli Ampere-Hour)  according to  the system requirement
* Rechargeable&#x20;
* Lightweight (which LIPOs already are)&#x20;

**State Indicator(s)**

Generally, LEDs and buzzers are used as state indicators

**Data Recorder**

**SD card** is one of the easiest ways to go but you can also use **Flash chips** which can be more reliable.&#x20;

The microcontrollers themselves also have flash memory but it's not enough to store a large number of readings.



These are all the various components that are used in the Avionics of the model rockets.

Now let's look at our first flight computer. Introducing **SNS v1**









\
\
