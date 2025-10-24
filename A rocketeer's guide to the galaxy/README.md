---
description: Introduction
cover:
  light: .gitbook/assets/2001_space_art.jpg
  dark: .gitbook/assets/2001_space_art.jpg
coverY: 0
layout:
  width: default
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# Introduction to Avionics and Guidance Systems

#### What is Avionics and Guidance system in Rockets?

If Propulsion is the heart of a rocket then Avionics is the brain and the nervous system.&#x20;

There are two major functions of the Avionics system of rocket

* Telemetry &#x20;
* Guidance and Navigation

#### What is Telemetry?

Telemetry is simply the collection of data of a wide range of parameters provided by the array of sensors that are present in the rocket, its real-time transmission, and analysis of the data received.

This leads us to question what are the different parameters that are to be measured on a rocket are what are the variety of sensors that are required for that.

* There are large no of sensors that are present in a rocket system,&#x20;
  * Inertial Measurement Units (IMUs)
  * Altitude Sensors
  * Pressure Sensors
  * Temperature Sensors
  * Strain Gauges
  * Flow Sensors&#x20;
  * Vibration Sensors
  * Radiation Detectors
  * Navigation Sensors
  * Cameras and Imaging sensors

Data is collected from these sensors constantly the data gathered is then streamed with the help of communication systems on board.

High-quality RF communication is used to stream and receive data from rockets.

The real-time data received is used for _Trajectory analysis, Performance Monitoring, Safety checks, and health checks_ of the rocket.

#### What is a Guidance and Navigation system?

notes:

1. One of the important things about rockets is that they should have a controlled flight with a defined trajectory nai to rocket to Diwali waala bhi hota hai.
2. Are rockets controlled by humans/manually?

A rocket almost never flies manually they have a predefined course that is programmed into the system and the flight is done autonomously accordingly.

In Guidance and Navigation systems the data about where the rocket is in what orientation, at what speed, and heading in which direction is acquired from all the onboard sensors we talked about. Majorly with the help of _Inertial Measurement Units and_ _GPS systems._\


The data received is then further used to guide the rocket with the help of a flight control system. \


#### Flight Control System

A rocket is pre-programmed for its destination.&#x20;

A flight algorithm is written such that the data is received from the guidance sensors and fed into the algorithm which then calculates things like the rocket's &#x4F;_&#x72;ientation_, _Speed,_ and _further trajectory._&#x20;

_How can a rocket be oriented to follow its trajectory?_&#x20;

Two widely used techniques for Active control of rockets are:&#x20;

* Thrust vector control&#x20;
* Actuating Fins control&#x20;

**What is Thrust Vector Control?**

It is a technique to orient a rocket (Draw and explain vectors).

There are quite a few methods that can be used in thrust vectoring.

1. The most commonly used is gimbaling  a motor or nozzle of the rocket&#x20;
2. Jet vanes. (kind of like actuating fins for propellent flown off the rocket)
3. LITVC (Liquid injection thrust vector control)\
   Injecting a reactive or inert gas into the exhaust stream we can change its direction.
4. Thrust paddle system (kind of like jet vanes just paddles instead)
5. Vernier thrusters (small thrusters that are mostly present in payload and use inert gases)

#### Actuating Fins Control&#x20;

Another method used for directing the rocket is fins actuation.

In this method, there are Fins controlled by servo motors to orient a rocket by deflecting the airflow.
