https://vimeo.com/661053454

### Synchronous Serial Protocols
The synchronous type of serial protocols such as SPI, I2C, CAN and LIN are used in different projects because it is one of the best resources for onboard peripherals. Also these are the widely used protocols in major applications.

#### SPI Protocol

The Serial Peripheral Interface (SPI) is a synchronous interface that allows several SPI microcontrollers to be interconnected. In SPI, separate wires are required for data and clock lines. Also the clock is not included in the data stream and must be furnished as a separate signal. 

The SPI can deliver up to 10Mbps of speed and is ideal for high-speed data communication.

#### I2C Serial Communication

Inter integrated circuit (I2C) two-line communication between different ICs or modules, where the two lines are SDA (Serial Data Line) and SCL (Serial Clock Line). Both the lines must be connected to a positive supply using a pull up resistor. I2C can deliver speed up to 400Kbps, and it uses 10 bit or 7 bit addressing system to target a specific device on the I2C bus, so it can connect upto to 1024 devices.

#### USB

USB (Universal Serial Bus) is a widely used protocol with different versions and speeds. A maximum of 127 peripherals can be connected to a single USB host controller. USB acts as a "plug and play" device. The USB is used in almost all devices such as keyboards, printers, media devices, cameras, scanners, mouse etc. It is designed for easy installation, faster data rate, less cabling and hot-swapping.

#### CAN

The Controller Area Network (CAN) is used in automotive applications to allow communication between ECUs (Engine Control Units) and sensors. The CAN protocol is robust, low-cost and message-based and covers many applications, e.g. cars, trucks, tractors, industrial robots etc. The CAN bus system allows for central error diagnosis and configuration across all ECUs. CAN messages are prioritized via IDs so that the highest priority IDs are non-interrupted. Each ECU contains a chip for receiving all transmitted messages, deciding relevance and acting accordingly. This allows easy modification and inclusion of additional nodes (e.g. CAN bus data loggers).

### Asynchronous Serial Protocols
The asynchronous type of serial protocol is very essential when it comes to long-distance reliable data transfer. This does not require a timing clock that is common to both devices. Each device independently listens and sends digital pulses that represent bits of data at an agreed-upon rate. 

Asynchronous serial communication is sometimes referred to as Transistor-Transistor Logic (TTL) serial.

#### 1.RS232

The RS232 (Recommended Standard 232) is a very common protocol used to connect different peripherals such as monitors, CNC machines etc. The RS232 comes in male and female connectors. The RS232 is a point-to-point topology with a maximum of one device connected and covers a distance up to 15 meters at 9600 bps.

#### 2. RS422

The RS422 is similar to RS232 which allows to simultaneously send and receive messages on separate lines but uses a differential signal for this. In the RS-422 network, there can only be one transmitting device and up to 10 receiving devices. The data transfer speed in RS-422 depends on the distance and can vary from 10 kbps (1200 meters) to 10 Mbps (10 meters).

#### 3. RS485

Since RS485 uses multi-point topology, it is mostly used in the industries and is an industry preferred protocol. RS422 can connect 32 line drivers and 32 receivers in a differential configuration, but with the help of additional repeaters and signal amplifiers, it can handle up to 256 devices.

https://www.youtube.com/watch?v=IyGwvGzrqp8

If you are interested to learn more about CAN, here is a good resource:

[CAN Basics](https://automotivetechis.wordpress.com/2012/06/01/can-basics-faq/).