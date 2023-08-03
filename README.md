# I2C_Communication
Task 2 of the Internet of Things path:

This project is a communitation between two arduino's to turn on/off led using a button.


<img width="1080" alt="Screenshot 1445-01-16 at 4 43 27 PM" src="https://github.com/Ramahalharbi/I2C_Communication/assets/139393175/39efb15a-568d-4552-95b6-f6a226a3c2f9">






#I2C Serial Communications

I2C (Inter-Integrated Circuit) is a serial communication protocol that allows multiple devices to communicate with each other using just two wires. In an I2C communication setup, one device acts as the "master" and the other device(s) act as "slaves".

In your case, one Arduino board will act as the sender (master) and the other Arduino board will act as the receiver (slave). The sender will send data to the receiver over the I2C bus.

To set up I2C communication between two Arduinos, you will need to connect the two boards using two wires: SDA (serial data) and SCL (serial clock). These pins are usually labeled on the Arduino board.

The sender (master) will initiate communication by sending a start signal on the SDA line. This will let the receiver (slave) know that communication is starting. The master will then send the address of the slave it wants to communicate with, followed by the data it wants to send.

The slave will respond to the master's request and send an acknowledgment signal back to the master. The master will then continue sending data until it is finished, and then send a stop signal to end the communication.

