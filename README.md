# rpi-ultrasonic-servohat
Resources explaining how to use the ultrasonic sensor with the 16 channel servo hat for the raspberry pi.

![Ultrasonic Sensor hard wired to Servo HAT](pi-hat-with-ultrasonic-sensor.png?raw=true)


## Board Mode Setup Info

Adapted from https://tutorials-raspberrypi.com/raspberry-pi-ultrasonic-sensor-hc-sr04/

```Python
  #set GPIO Pins
  GPIO_TRIGGER = 40
  GPIO_ECHO = 38
 
  #set GPIO direction (IN / OUT)
  GPIO.setup(GPIO_TRIGGER, GPIO.OUT)
  GPIO.setup(GPIO_ECHO, GPIO.IN)
```  
 
## Using GPIO Zero Library Setup

Complete example: https://www.raspberrypi.org/learning/physical-computing-with-python/distance/

```Python
  ultrasonic = DistanceSensor(echo=20, trigger=21)
``` 
