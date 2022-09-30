# Feetech-Servo-SDK [![Platforms](https://img.shields.io/badge/Raspberry%20Pi-A22846?style=for-the-badge&logo=Raspberry%20Pi&logoColor=white)](https://img.shields.io/badge/Raspberry%20Pi-A22846?style=for-the-badge&logo=Raspberry%20Pi&logoColor=white) [![Language](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) [![IDE](https://img.shields.io/badge/PyCharm-000000.svg?&style=for-the-badge&logo=PyCharm&logoColor=white)](https://img.shields.io/badge/PyCharm-000000.svg?&style=for-the-badge&logo=PyCharm&logoColor=white) [![adam package](https://img.shields.io/badge/adam_package-red?style=for-the-badge&logo=python&logoColor=white)](https://github.com/Adam-Software)


[![License](https://img.shields.io/github/license/Adam-Software/Feetech-Servo-SDK.svg)](https://img.shields.io/github/license/Adam-Software/Feetech-Servo-SDK.svg)
[![PyPI version](https://badge.fury.io/py/feetech-servo-sdk.svg)](https://badge.fury.io/py/feetech-servo-sdk) 


This is source code from [official feetech repository](https://gitee.com/ftservo/SCServoSDK).
The repository structure copies the structure of the [original library](https://gitee.com/ftservo/SCServoSDK/blob/e4d07f43c4c34827b2e226cf5cc706576504ebeb/SCServo_Python_200831.7z)

## Structure

```
root dirrectory
     |---scservo_sdk 
     |---scsservo_sdk_example
```
The `scsservo_sdk_example` directories contain examples of using the library.

The source code of the library is located in the `scservo_sdk` directory.

The `scsservo_sdk_source` directory contains the original archive with the source code of the library from the developer.

## Usage

Tested on `Linux raspberrypi 5.15.61-v8+ #1579 SMP PREEMPT Fri Aug 26 11:16:44 BST 2022 aarch64`.
Python version `Python 3.9.2`.

### Method 1. Clone repositry

```
$ cd /usr/src/
$ sudo git clone https://github.com/Adam-Software/Feetech-Servo-SDK.git
$ sudo chown -R pi Feetech-Servo-SDK
$ cd Feetech-Servo-SDK/scsservo_sdk_example
$ python3 ping.py
Succeeded to open the port
Succeeded to change the baudrate
[ID:001] ping Succeeded. SCServo model number : 1540
```

### Method 2. Install pip package

Copy the sample file to any location convenient for you. In the example I use `/home/pi/FeetechTestFiles`

```
$ pip install feetech-servo-sdk
$ cd /home/pi/FeetechTestFiles
$ python3 ping.py
Succeeded to open the port
Succeeded to change the baudrate
[ID:001] ping Succeeded. SCServo model number : 1540
```
