# rpi-ultrasonic-servohat
Resources explaining one way to connect the ultrasonic sensor (HC-SR04) with the 16 channel servo hat for the raspberry pi.

Accompanying video: https://youtu.be/Xj3dXUahiXU

I could not draw the exact implementation shown in the video, since the resistors are vertical in the prototype.

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
 
## GPIO Zero Library Setup Info

Complete example: https://www.raspberrypi.org/learning/physical-computing-with-python/distance/

```Python
  ultrasonic = DistanceSensor(echo=20, trigger=21)
``` 
