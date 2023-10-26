# C-Projects

## C Serial Port Reader

This C program reads data from a serial port and displays it. It is configured to read from a specific serial port at a baud rate of 9600, without any parity checks and with 8 data bits. Hardware flow control (RTS/CTS) is disabled, and software flow control (XON/XOFF) is also disabled. The program reads one character at a time and waits for input indefinitely.

## Prerequisites

- Make sure to connect a device to the specified serial port (`/dev/ttyUSB0`).
- This program is intended for Unix-like operating systems.

## How to Use

1. Compile the program using your C compiler.

```bash
gcc serial_port_reader.c -o serial_port_reader
```
2. Execute the program:

```bash
./serial_port_reader
```

- The program will open the serial port, configure it, and start reading data. If data is received, it will be displayed on the console. If you want to stop the program, press `Ctrl+C`.
