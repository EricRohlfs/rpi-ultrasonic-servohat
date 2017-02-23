# rpi-ultrasonic-servohat
Resources explaining how to use the ultrasonic sensor with the 16 channel servo hat for the raspberry pi.


## Board Mode Setup Info

```Python
  #set GPIO Pins
  GPIO_TRIGGER = 40
  GPIO_ECHO = 38
 
  #set GPIO direction (IN / OUT)
  GPIO.setup(GPIO_TRIGGER, GPIO.OUT)
  GPIO.setup(GPIO_ECHO, GPIO.IN)
```  
 
## Using GPIO Zero Library Setup

  ultrasonic = DistanceSensor(echo=20, trigger=21)

