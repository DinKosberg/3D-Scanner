# Arduino LED Sequence Script

This repository contains a Python script for controlling a sequence of LEDs using an Arduino board. The script is written in Python and uses the `pyfirmata` library to communicate with the Arduino.

## Description

The script connects to an Arduino board via a specified COM port (COM3 in this case) and initializes four LEDs connected to digital pins 10, 11, 12, and 13. The LEDs are controlled in a sequence, each representing a bit in a binary count from 0 to 15. The sequence repeats indefinitely until the program is manually terminated.

## Prerequisites

To run this script, you will need:

- An Arduino board
- Four LEDs connected to the Arduino's digital pins 10, 11, 12, and 13
- Python 3.x installed on your computer
- The `pyfirmata` Python library

## Installation

1. **Install Python**:
   - Download and install Python from [python.org](https://www.python.org/downloads/).

2. **Install pyfirmata**:
   - Install the `pyfirmata` library using pip:
     ```
     pip install pyfirmata
     ```

3. **Setup Arduino**:
   - Connect the LEDs to the Arduino board on the specified pins.
   - Connect the Arduino to your computer via USB.

4. **Clone the Repository**:
   - Clone this repository to your local machine or download the script.

## Usage

1. **Connect the Arduino**:
   - Ensure the Arduino board is connected to your computer and to the correct COM port (COM3 by default).

2. **Run the Script**:
   - Navigate to the script's directory in your terminal.
   - Run the script using Python:
     ```
     python led_sequence.py
     ```

3. **Observe the LED Sequence**:
   - The LEDs will light up in a binary counting sequence from 0 to 15.
   - The count is printed to the console.

## Modifying the Script

- To change the COM port, modify the `board = Arduino('COM3')` line with the appropriate port.
- The `wait` variable can be adjusted to change the speed of the LED sequence.

## Contributing

Feel free to fork the repository and submit pull requests with any enhancements or bug fixes.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
