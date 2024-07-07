# Design-and-programming-an-ESP-circuit-with-a-sensor
This project is an electronic circuit using an ESP32 development panel with an ultrasonic distance control sensor (HC-SR04).


<img width="1710" alt="‏لقطة الشاشة ١٤٤٦-٠١-٠٢ في ١٢ ٣٥ ٤٠ ص" src="https://github.com/ijana7/Design-and-programming-an-ESP-circuit-with-a-sensor/assets/173642526/a346af7c-dea0-4e5d-a5c0-d7cad181ac08">

## the link

https://wokwi.com/projects/402788800054477825

## code explain

In the `loop()` function, which runs continuously:
   - It first clears the `trigPin` to make sure no old signal is present.
   - Then, it sends a short high pulse (10 microseconds) to the `trigPin`. This triggers the ultrasonic sensor to send out a sound wave.
   - The program then waits for the sound wave to bounce back and be detected on the `echoPin`. It measures the time it takes for the sound wave to travel to the object and back.
   - Using the time measurement, the program calculates the distance to the object in centimeters.
   - Finally, it prints the calculated distance to the serial monitor.

 The program pauses for 500 milliseconds (half a second) before repeating the process.

## The key steps are:
1. Trigger the sensor to send out a sound wave.
2. Measure the time it takes for the sound wave to bounce back.
3. Calculate the distance based on the time measurement.
4. Display the distance on the serial monitor.

This process continues in a loop, allowing the Arduino to continuously monitor the distance to an object in front of the ultrasonic sensor.
