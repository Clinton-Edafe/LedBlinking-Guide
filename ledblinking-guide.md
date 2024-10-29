# How to Adjust the Blinking Speed of the LED

## Table of Contents
- [Objective](#objective)
- [Steps](#steps)
  - [1. Open the Code in the Arduino IDE](#1-open-the-code-in-the-arduino-ide)
  - [2. Locate the delay(1000); Lines in the Code](#2-locate-the-delay1000-lines-in-the-code)
  - [3. Change the Delay Value](#3-change-the-delay-value)
  - [4. Upload the Updated Code to the Arduino](#4-upload-the-updated-code-to-the-arduino)
  - [5. Observe the Change in Blinking Speed](#5-observe-the-change-in-blinking-speed)

---

## Objective
Learn how to modify the delay time in the code to change the LED's blinking speed.

---

## Steps

### 1. Open the Code in the Arduino IDE

Open the Arduino IDE on your computer and load the LED blinking code.

---

### 2. Locate the `delay(1000);` Lines in the Code

Find the lines in the code that contain `delay(1000);`. These lines control the timing of the LED's on and off states.

---

### 3. Change the Delay Value

- **Increase the delay** value (e.g., `delay(2000);`) to slow down the blinking speed.
- **Decrease the delay** value (e.g., `delay(500);`) to speed up the blinking.

---

### 4. Upload the Updated Code to the Arduino

Once you've modified the delay values, upload the code to your Arduino board.

---

### 5. Observe the Change in Blinking Speed

After the code is uploaded, the LED should blink at the new speed according to your modified delay value.

---

### Visual Representation of Delay Change Impact

Below is a diagram that shows how adjusting the `delay()` value changes the LED's blinking pattern. Increasing the delay results in slower blinking, while decreasing the delay causes faster blinking.

```mermaid
sequenceDiagram
    participant A as Arduino
    participant LED as LED

    A->>LED: Turn ON (digitalWrite(HIGH))
    LED-->>A: Waiting (delay(2000ms))
    A->>LED: Turn OFF (digitalWrite(LOW))
    LED-->>A: Waiting (delay(2000ms))
    A->>LED: Turn ON (digitalWrite(HIGH))
    LED-->>A: Waiting (delay(500ms))
    A->>LED: Turn OFF (digitalWrite(LOW))
    LED-->>A: Waiting (delay(500ms))