Setup the RPi:  
sudo apt-get install build-essential python3-dev python-smbus i2c-tools python3-pip --yes

Activate I2C in raspi-config  
Check it: i2cdetect -y 1  

sudo pip3 install Adafruit-PCA9685  

PCA9685	I2C Servo Board  
SCL	GPIO 3 -> RPi SCL Pin 5  
SDA	GPIO 2 ->  RPi SDA Pin 3  
VCC / V	3,3V -> RPi Pin 1  
GND	GND (Pin 6)  

TBC
