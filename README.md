# Accelerometer and GPIO activation in RK-Development Board

In this script, I took lsm6dsx sensor driver from Android source code and I edited it. I added GPIO to check if their value is changing while angle of axis is changing. To see that more clearly I added some LED's and they will blink if specific angle is reached. Then I added GPIO's in device tree file to make it more easier to change GPIO's value and number. To do this I created a device tree parser function to make it easier. Proccess will be activated when device boots up. To make it possible I added a thread to read X axis and Y axis values continuously. To see more clearly which led is blinking, I added threshold in thread.

### How to run the project:

To run the project you need to build OS and flash it to your device. Device is RK3399-Excavator-Sapphire-Development-Board