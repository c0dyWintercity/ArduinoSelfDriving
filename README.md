# ArduinoSelfDriving
This tutorial uses an ultrasonic sensor to turn any car with motor into AI. This is a great learning experience for anyone to get started in learning robotics.


# Materials Needed: 
- soldering iron
- hot glue gun
- Elegoo Smart Car 3.0
- **optional:** *instead of getting the whole car kit:* (L298N[motors],Arduino UNO[main board])
- rc car
- pc/laptop/raspberry pi

# Notes:
- On my car, the front motor controls steering, while the rear controls speed

# Step One (building):

- pos and neg for rear motor to IN1 on L298N
- pos and neg for front motor to IN3 on L298N
- pos and neg for power source
- L298N is controlled with 6 pins. ENA and ENB, both control the amount of power (yes PWM capable) to each motor. ENA controls IN1/IN2. ENB controls IN2/IN4. IN1/IN2 are digital outputs allowing to forward/reverse. IN3/IN4 are digital outpurs allowing to turn left/right. 
- **L298N_Control pins:**
- ENA->6 ; IN1->11 ; IN2->9 ; IN3->8 ; IN4->7 ; ENB->5
- If you decide to buy the car kit, it comes with a sheild that labels everything beautifully. 
- **Ultrasonic Sensor pins:**
- VCC->5V ; Trig->A5 ; Echo->A4 ; GND->GND

# Step Two (Code):

- Download the Arduino IDE
- upload one of the .ino files provided
- have fun! 


I have to give credit where it's due. They are changed quite a bit, but the .ino files are based off the code Arduino had open-sourced for it's Elegoo Smart Car 3.0. 







