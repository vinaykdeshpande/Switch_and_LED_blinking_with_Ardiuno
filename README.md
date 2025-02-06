# Switch_and_LED_blinking_with_Ardiuno

This project controls an LED using a button on an Arduino board. Each button press changes the LED's blinking speed.

1.  **What This Program Does**
  - **Press the button** to change the LED blinking speed:
  - **1st Press:** LED blinks every 1 second (0.5 Hz)
  - **2nd Press:** LED blinks every 0.5 seconds (1 Hz)
  - **3rd Press:** LED blinks every 0.25 seconds (2 Hz)
  - **4th Press:** LED turns OFF
  - **5th Press:** Repeat the 1st step

2.   **Hardware Setup:**
  - **LED (Pin 13)**: Connect an LED with a resistor to pin 13.
  - **Button (Pin 2)**: Connect a button to pin 2 with a pull-down resistor or use the internal pull-up.

3.  **Assumptions Made**
  - The **LED is connected to pin 13**.
  - The **Button is connected to pin 2** and uses the **internal pull-up resistor**.
  - **Debouncing** is handled with a **200 ms delay** to prevent false button presses.
  - The program uses **non-blocking timing** with the `millis()` function.
