# AVR Code for Aqua Culture Fish Feeder System

This directory contains the AVR code for the Aqua Culture Fish Feeder System, which monitors and controls environmental parameters in an aquaculture tank using an ATmega328P microcontroller. The code includes functionality for an LCD display, sensor readings for temperature, pH, and TDS (Total Dissolved Solids), motor control for fish feeding, and a button-based menu system.

## Features

- **LCD Display Control**: Utilizes an I2C 16x2 LCD to display sensor readings and system status.
- **Temperature Sensing**: Interfaces with a DS18B20 sensor to monitor water temperature.
- **TDS and pH Monitoring**: Reads and displays water quality using analog TDS and pH sensors.
- **Motor Control**: Operates a feeding motor based on user settings and schedules.
- **User Interface**: Provides a simple button-driven menu for setting parameters and manual control.

## File Overview

- **main.c**: The main application code that initializes all peripherals and manages the main program loop.
- **Functions for LCD**: Functions and definitions for controlling the I2C LCD display.
- **ds18b20**: Functions for interfacing with the DS18B20 temperature sensor.
- **tds & pH**: Code for reading TDS and pH sensor values.
- **motor control**: Functions for controlling the feeding motor.
- **menu**: Implements the user interface for navigating the menu and setting parameters.

## Installation

To compile and upload the AVR code to the ATmega328P microcontroller:

1. **Clone this repository**:
    ```bash
    git clone https://github.com/yourusername/aqua-culture-fish-feeder.git
    cd aqua-culture-fish-feeder/avr_code
    ```

2. **Open in AVR Development Environment**:
   - You can use Atmel Studio, Arduino IDE, or any AVR-compatible IDE.
   
3. **Compile the Code**:
   - Ensure all necessary libraries and header files are included.
   - Set the microcontroller to ATmega328P and the correct clock speed (e.g., 16 MHz).

4. **Upload the Code**:
   - Connect your ATmega328P microcontroller to your computer via an AVR programmer or Arduino board.
   - Upload the compiled code to the microcontroller.

## Usage

1. **Power on the system** and observe the initialization messages on the LCD display.
2. **Navigate the menu** using the connected buttons to configure settings such as feeding times and sensor thresholds.
3. **Monitor the sensors**: Temperature, pH, and TDS readings will be continuously displayed on the LCD.
4. **Control the motor**: Use the menu to manually activate the feeding motor or set automated feeding schedules.

## Contributing

Feel free to contribute to the project by forking the repository, making changes, and submitting a pull request. For significant changes, please open an issue first to discuss your ideas.

## License

This code is open-source and available under the MIT License. See the [LICENSE](LICENSE) file for more information.
