# *Water Level Controller Using 8051 Microcontroller*

The water level controller detects the water level in a tank to assist in automatically controlling the water motor. It does this by utilizing the 8051 microcontroller project. In this post, you will learn how to monitor and control water levels in tanks and other containers. This device monitors the tank's water level and activates the motor when it is empty.

When the top tank, or tanky, is full, the motor is turned off. Here, the LCD screen (liquid crystal display) displays the tank's water level. We can also prevent the water from overflowing by using this approach. Here, we are developing the circuit that uses an 8051 microcontroller to automatically monitor and regulate the water level in the overhead tank.

## *Introduction*

The term "water level controller" refers to an electronic device or circuit package that controls the water level. Water level controllers play a crucial role in managing water resources effectively, preventing both the overflow and depletion of water in tanks. It is difficult to know the level of water in the overhead tank such that wastage of water can happen frequently. To conserve water, avoid overflow of water in the overhead tank which may cause loss of water, loss of electrical power, etc.,. Thus, an ultrasonic water level controller using 8051 microcontroller is an innovative electronics project application for controlling water level.

Water Level Controller using 8051 Microcontroller project will help in automatically controlling the water motor by sensing the water level in a tank. This article explains how to detect and control the water level in an overhead tank or any other container. This system monitors the water level of the tank and automatically switches ON the motor whenever tank is empty. 

## *Motivation*
A water level controller is a device that manages water levels on a variety of systems such as water tanks, pumps and swimming pools. The basic function of a water level controller is to regulate water flow and optimize system performance. One of the main advantages of water level control devices includes the ability to control power fluctuations when the motor is switched on. Most of these devices ensures uninterrupted water supply by filling the overhead tank once it is below level. The motor power is switched on when the overhead tank becomes empty and switches off automatically when the underground tank is empty or the 
overhead tank becomes full. In this way it becomes easy to ensure 24 hours water supply without any kind of interruption.

## *Applications*
- It is used in like applications like storage, tank, boilers e.t.c. to indicate the level of water inside.
- It can be used to calculate incoming and outgoing water in large reservoirs.
- Fuel level indicator in vehicles.
- It can be used to measure underground storage of water.
- Used in big buildings where manual monitoring is difficult.
- Used in industries to control the liquid level automatically.
- Automatic water level controllers can be used in Homes apartments, commercial complexes.

## *Advantages*
- Easy to install.
- Very little maintenance.
- Compact design.
- Automatic water level indicators ensure no overflows or running of dry pumps.
- Saves money by using less water and electricity.
- Can help avoid seepage of walls and roofs due to tanks overflowing.


## *Limitations*
- The Rust, Foul and Deteriorate.
- Wire use in the tank can be replaced every two years.

**System Circuit Diagram**
| :--: |
![CIRCUIT DIAGRAM](https://github.com/user-attachments/assets/aa4162f3-7aaa-4a53-9b26-b1925ab7f122)

## *Component Used*
- AT89S52 Microcontroller (or any 8051 based Microcontroller)
- 8051 Programmer (Programming Board)
- 11.0592 MHz Quartz Crystal
- 2 x 33pF Capacitor
- 2 x 10KΩ Resistor (1/4 Watt)
- 10µF Capacitor
- Push Button
- 1KΩ x 8 Resistor Pack (for Pull – up)
- 16 x 2 LCD Display
- 5V Relay
- 4 x 2N2222 (NPN) Transistors
- DC Motor (for demonstration)
- 10KΩ Potentiometer
- 1N4007 PN Junction Diode
- Programming cable
- Connecting wires
- Power Supply
- Keil µVision IDE
- Proteus (for circuit diagram)

## *Algorithm for Water Level Controller Circuit*
``` ruby
1) First, set the controller pins P0.0, P0.1, and P0.2 to inputs and P0.7 to output. Initialize the LCD now.
2) Check the input pins P0.0, P0.1, and P0.2 for water level continuously.
3) If all of the pins are low, the tank will be displayed as "EMPTY" on the LCD, and the P0.7 pin will be set to HIGH to automatically operate the motor.
4) Show the water level as "LOW" and keep the motor running if the level is low, that is, if P0.0 is HIGH.
5) Half level water is indicated by a HIGH pulse on pin P0.1. Thus, run the motor normally while displaying the same content on the LCD.
6) It indicates that the tank's water level is FULL if P0.2 is HIGH.
7) At this point, set the P0.7 pin to LOW to turn the motor off automatically.
```

## *Operating Mechanism of Water Level Controller*
``` ruby
Step 1 - Initialize the system 
Step 2 - Check whether the underground tank is full or not
Step 3 - If water in upper tank is below lower sensor, turn on the motor and display the message ‘Tank is empty and Motor is on’.
Step 4 - If water in upper tank is above lower sensor and below the mid sensor, turn on the motor and display the message ‘Tank is empty and Motor is on’.
Step 5 - If water in upper tank touches the upper sensor, turn off the motor and display the message ‘Tank is full and motor is off’.
```

## *Results*

### Simulation Result State - 1

![TANK IS EMPTY](https://github.com/user-attachments/assets/6fc368f4-19a7-472c-ad39-a5a4c1ce640b)
| :--: |
**TANK IS EMPTY AND MOTOR IS ON**

### Simulation Result State - 2

![TANK FILLING](https://github.com/user-attachments/assets/186e57da-17a6-4090-8644-5bbfccc0293c)
| :--: |
**TANK FILLING AND MOTOR IS ON**

### Simulation Result State - 3

![TANK IS MID](https://github.com/user-attachments/assets/ee0a1a81-2ffb-46d1-b4ca-fccc696762f8)
| :--: |
**TANK IS MID AND MOTOR IS ON**

### Simulation Result State - 4

![TANK IS FULL](https://github.com/user-attachments/assets/b022212e-43e2-4ca2-ad1d-4812d1b02932)
| :--: |
**TANK IS FULL AND MOTOR IS OFF**

## *Conclusion*
- This type of water level controller will reduce the human interference. The power consumption of the motor and the wastage of water because of unwanted overflow can be controlled.
- The whole system operates automatically. So it does not need any expert person to operate it. It is not so expensive. This design has much more scope for future research and development.

## *Future scope*
- Automatic water level monitoring system has a good scope in future especially for agriculture sector. There are any areas where we need water level controller. It could be agricultural fields, overhead tanks. We can make this project wireless by using NRF transmitter and receiver.
- In this system, future modifications can also be done like interface of GSM module to send SMS alerts to the user.
- 
## *References*
- https://www.electronicshub.org/water-level-controller-using-8051-microcontroller/
- http://www.circuitstoday.com/water-level-controller-using-8051
