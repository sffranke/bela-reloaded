Download Buster Image  
touch ssh in /boot of image    
vi /boot/wpa_supplicant.conf  
->  
country=DE # Your 2-digit country code  
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev  
network={  
    ssid="YOUR_NETWORK_NAME"  
    psk="YOUR_PASSWORD"  
    key_mgmt=WPA-PSK  
}  
  

Setup the RPi:  
sudo apt-get install build-essential python3-dev python3-smbus i2c-tools python3-pip --yes

Activate I2C in raspi-config  
Check it: i2cdetect -y 1  

sudo pip3 install Adafruit-PCA9685

sudo pip3 install pygame for ps4 controller  

sudo apt-get dist-upgrade -y  
sudo apt-get install pi-bluetooth  
sudo apt-get install bluez bluez-firmware
sudo usermod -G bluetooth -a pi
sudo reboot



sudo bluetoothctl  
agent on  
default-agent  
scan on  

sudo dd if=/dev/disk1 of=/Users/myaccount/Pibackup.dmg  :-)  
Restore:  
diskutil unmountDisk /dev/disk2  
sudo dd if=/Users/myaccount/Pibackup.dmg of=/dev/disk2  

PCA9685	I2C Servo Board  
SCL	GPIO 3 -> RPi SCL Pin 5  
SDA	GPIO 2 ->  RPi SDA Pin 3  
VCC / V	3,3V -> RPi Pin 1  
GND	GND (Pin 6)  

MPU-6050 connected to I2C bus.  

TBC
