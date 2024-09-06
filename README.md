# Potentiometer-Controlled LED Brightness on Arduino

This project demonstrates how to control the brightness of an LED using a potentiometer. The analog input from the potentiometer is mapped to control the PWM output, adjusting the LED brightness accordingly.

## Components Used

- Arduino Uno
- Potentiometer (connected to analog input A0)
- LED (connected to digital pin 11)
- Resistors
- Wires
- Breadboard

## How It Works

- The potentiometer provides an analog input to pin A0, which ranges from 0 to 1023.
- The analog value is mapped to a PWM value (0 to 255) using the `map()` function.
- The PWM value is sent to the LED on pin 11, adjusting its brightness.

## Pin Configuration

- **Potentiometer**:
  - Center pin connected to A0 (analog input)
  - Other two pins connected to 5V and GND
- **LED**:
  - Positive leg connected to pin 11 (PWM output)
  - Negative leg connected to GND (via a resistor)

## Code Explanation

- The potentiometer value is read using `analogRead()` from pin A0.
- The value is then mapped from its range of 0-1023 to 0-255 (suitable for PWM).
- The `analogWrite()` function is used to send the mapped PWM value to the LED, adjusting its brightness in real-time based on the potentiometer's position.

## How to Use

1. Connect the potentiometer and LED according to the pin configuration.
2. Upload the provided code to your Arduino board.
3. Turn the potentiometer to adjust the LED's brightness.
   - Turning the potentiometer will increase or decrease the brightness in a smooth transition.

## Features

- Smooth brightness control of the LED using a potentiometer.
- Real-time interaction with analog input and PWM output.
- Easy-to-understand implementation for beginners.

## License

This project is open-source and can be modified or distributed freely.
