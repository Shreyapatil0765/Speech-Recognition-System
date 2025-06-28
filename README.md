*Company*: CODTECH IT SOLUTIONS

*NAME*: SHREYA PATIL

*INTERN ID*: CT04DF2846

*DOMAIN*: EMBEDDED SYSTEMS

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTOSH


# Speech-Recognition-System

This project involves the development of a Speech Recognition System, an embedded solution designed to control a lamp and a fan using voice commands transmitted via Bluetooth. The main objective is to enhance user convenience by enabling hands-free control of appliances, while also showcasing the integration of embedded systems with wireless communication.
________________________________________

Project Components 

The key components of this system include:

1.	Arduino Uno: A widely-used microcontroller board that acts as the core processing unit, interpreting signals and triggering the appropriate actions.
2.	Bluetooth Module (HC-05/06): Facilitates wireless communication between the Arduino and a smartphone. It receives signals generated from voice commands through a mobile app.
3.	Relay Modules: These act as switches that safely control the AC power to the lamp and fan, isolating the low-voltage Arduino from high-voltage circuits.
4.	Lamp and Fan: The end devices that are toggled ON/OFF based on voice inputs processed by the system.
________________________________________

System Operation and Design 

The Speech Recognition System allows the user to control household appliances through spoken instructions. The process is as follows:

1.	A custom Android application, developed using MIT App Inventor, listens to the user's voice command.
2.	The app translates the spoken command (like “Turn on light” or “Turn off fan”) into Bluetooth signals.
3.	These signals are wirelessly transmitted to the Bluetooth module connected to the Arduino Uno.
4.	Based on the received command, the Arduino decides which appliance to operate:
i.	Pin 10 is connected to a relay controlling the lamp.
ii.	Pin 8 is connected to a relay controlling the fan.
5.	When triggered, each relay allows current to flow to the corresponding appliance, thereby switching it ON or OFF.

Relays are used for their ability to electrically isolate the control circuitry from the appliance power supply, ensuring the safety and integrity of the microcontroller during operation.
________________________________________

Software and Development Tools

Two primary software platforms were employed in the development of this project:

1. Arduino IDE: Used for writing, compiling, and uploading the embedded code to the Arduino Uno. It handles serial communication, processes received data, and controls the output pins.
2. MIT App Inventor: A drag-and-drop, visual programming platform used to build the Android application. It captures voice input, converts it to text, and transmits corresponding commands via Bluetooth.
3. 
This pairing enables a seamless bridge between mobile user input and microcontroller-based hardware control.
________________________________________

System Architecture

The architecture of the Speech Recognition System follows a straightforward yet effective design:

1.	User gives a voice command via a smartphone.
2.	The MIT App Inventor app interprets the voice and converts it into Bluetooth-compatible data.
3.	The Bluetooth module receives this data and forwards it to the Arduino Uno.
4.	The Arduino deciphers the command and activates the appropriate relay.
5.	The relay then toggles the connected appliance (lamp or fan) ON or OFF.
This architecture promotes efficient communication between the user and devices, highlighting the practical fusion of embedded systems and mobile interfaces.
________________________________________

Future Enhancements

Some possible future improvements for the system include:

1.	Expanding support for multiple appliances using additional relay channels.
2.	Integrating Wi-Fi control via an ESP8266 or ESP32 for remote operation over the internet.
3.	Adding feedback mechanisms (like status LEDs or smartphone notifications) to confirm the current state of the appliances.
4.	Introducing AI-based voice assistants for more natural and multilingual interaction.


