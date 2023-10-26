# C Serial Port Reader

This C program reads data from a serial port and displays it. It is configured to read from a specific serial port at a baud rate of 9600, without any parity checks and with 8 data bits. Hardware flow control (RTS/CTS) is disabled, and software flow control (XON/XOFF) is also disabled. The program reads one character at a time and waits for input indefinitely.

## Prerequisites

- Make sure to connect a device to the specified serial port (`/dev/ttyUSB0`).
- This program is intended for Unix-like operating systems.

## How to Use

### Reading GPS data

1. Compile the program using your C compiler.

```bash
gcc gps.c -o gps_exe
```
2. Execute the program:

```bash
./gps_exe
```

### Reading RFID data

1. Compile the program using your C compiler.

```bash
gcc rfid.c -o rfid_exe
```
2. Execute the program:

```bash
./rfid_exe
```

- Both the program will open the serial port, configure it, and start reading data. If data is received, it will be displayed on the console. If you want to stop the program, press `Ctrl+C`.

## Configuration

- The program's configuration includes settings for:
  - Serial port: `/dev/ttyUSB0`
  - Baud rate: 9600
  - Data bits: 8
  - Parity: None
  - Stop bits: 1
  - Flow control: None

## Errors

If an error occurs during the execution, such as failing to open the serial port or reading serial data, the program will display an error message and terminate.

Feel free to modify the program or its configuration to suit your specific needs.

### Note:

This program is provided as-is and may require adjustments for your particular use case.
