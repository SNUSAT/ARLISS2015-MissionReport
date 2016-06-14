# Software System Code Manual

##1. Change log

|ISS/REV |	Date |	Modifications |	Created/modified by |
| -- | -- | -- | -- |
|1/0 |	11/20/2015 |	Codes upload(not edited) |	Hwijae Kwon gnlwo8599@gmail.com |

## 2. Codes
* These are our source codes. Some of them are made by ourselves, and some of them are from Github. We edited them to use for our project.


###1. IMU.h 
```cpp
1.	#ifndef IMU_h  
2.	#define IMU_h  
3.	  
4.	#include "Arduino.h"  
5.	#include <Wire.h>  
6.	  
7.	#define WHO_AM_I 0x01  
8.	#define REV_ID_MAJOR 0x02  
9.	#define REV_ID_MINOR 0x03  
10.	#define STATUS 0x04  
11.	#define I_ACC_X_LOW 0x10  
12.	#define I_ACC_X_HIGH 0x11  
13.	#define I_ACC_Y_LOW 0x12  
14.	#define I_ACC_Y_HIGH 0x13  
15.	#define I_ACC_Z_LOW 0x14  
16.	#define I_ACC_Z_HIGH 0x15  
17.	#define I_GYRO_X_LOW 0x16  
18.	#define I_GYRO_X_HIGH 0x17  
19.	#define I_GYRO_Y_LOW 0x18  
20.	#define I_GYRO_Y_HIGH 0x19  
21.	#define ADDRESS 0x20  
22.	#define I_GYRO_Z_LOW 0x1A  
23.	#define I_GYRO_Z_HIGH 0x1B  
24.	#define I_MAGNET_X_LOW 0x1C  
25.	#define I_MAGNET_X_HIGH 0x1D  
26.	#define I_MAGNET_Y_LOW 0x1E  
27.	#define I_MAGNET_Y_HIGH 0x1F  
28.	#define I_MAGNET_Z_LOW 0x20  
29.	#define I_MAGNET_Z_HIGH 0x21  
30.	#define C_ACC_X_LOW 0x22  
31.	#define C_ACC_X_HIGH 0x23  
32.	#define C_ACC_Y_LOW 0x24  
33.	#define C_ACC_Y_HIGH 0x25  
34.	#define C_ACC_Z_LOW 0x26  
35.	#define C_ACC_Z_HIGH 0x27  
36.	#define C_GYRO_X_LOW 0x28  
37.	#define C_GYRO_X_HIGH 0x29  
38.	#define C_GYRO_Y_LOW 0x2A  
39.	#define C_GYRO_Y_HIGH 0x2B  
40.	#define C_GYRO_Z_LOW 0x2C  
41.	#define C_GYRO_Z_HIGH 0x2D  
42.	#define C_MAGNET_X_LOW 0x2E  
43.	#define C_MAGNET_X_HIGH 0x2F  
44.	#define C_MAGNET_Y_LOW 0x30  
45.	#define C_MAGNET_Y_HIGH 0x31  
46.	#define C_MAGNET_Z_LOW 0x32  
47.	#define C_MAGNET_Z_HIGH 0x33  
48.	#define TEMPERATURE_LOW 0x34  
49.	#define TEMPERATURE_HIGH 0x35  
50.	#define ROLL_LOW 0x36  
51.	#define ROLL_HIGH 0x37  
52.	#define PITCH_LOW 0x38  
53.	#define PITCH_HIGH 0x39  
54.	#define YAW_LOW 0x3A  
55.	#define YAW_HIGH 0x3B  
56.	#define QUATERNION_X_LOW 0x3C  
57.	#define QUATERNION_X_HIGH 0x3D  
58.	#define QUATERNION_Y_LOW 0x3E  
59.	#define QUATERNION_Y_HIGH 0x3F  
60.	#define QUATERNION_Z_LOW 0x40  
61.	#define QUATERNION_Z_HIGH 0x41  
62.	#define QUATERNION_W_LOW 0x42  
63.	#define QUATERNION_W_HIGH 0x43  
64.	  
65.	  
66.	class IMU{  
67.	public:  
68.	  
69.	   IMU();  
70.	   int renew();  
71.	   void initiate();  
72.	   double getWHO_AM_I();  
73.	   double getSTATUS();  
74.	  
75.	   //double Status();  
76.	   double getRoll();  
77.	   double getPitch();  
78.	   double getYaw();  
79.	   double getGyroX();  
80.	   double getGyroY();  
81.	   double getGyroZ();  
82.	   double getAccX();  
83.	   double getAccY();  
84.	   double getAccZ();  
85.	   double getTem();  
86.	   String getSYaw();  
87.	   String getSGyroZ();  
88.	     
89.	  
90.	   uint8_t readRegister8(uint8_t Reg, double ft);  
91.	  
92.	private:  
93.	    
94.	   double status;  
95.	   double who_am_i;  
96.	   double Status;  
97.	  
98.	   double roll;  
99.	   double rollL;  
100.	double rollH;  
101.	  
102.	double pitch;  
103.	double pitchL;  
104.	double pitchH;  
105.	  
106.	double yaw;  
107.	double yawL;  
108.	double yawH;  
109.	     
110.	double gyroX;  
111.	double gyroXL;  
112.	double gyroXH;  
113.	  
114.	double gyroY;  
115.	double gyroYL;  
116.	double gyroYH;  
117.	  
118.	double gyroZ;  
119.	double gyroZL;  
120.	double gyroZH;  
121.	     
122.	double accX;  
123.	double accXL;  
124.	double accXH;  
125.	  
126.	double accY;  
127.	double accYL;  
128.	double accYH;  
129.	  
130.	double accZ;  
131.	double accZL;  
132.	double accZH;  
133.	  
134.	double temperature;  
135.	double temperatureL;  
136.	double temperatureH;  
137.	};  
138.	  
139.	#endif  
```

