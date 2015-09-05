## Adafruit Unified Sensor Library Unified L3G4200D Driver ##

This library was copied from Adafruit's LG3D20 unified libraray.  All I had available at the moment was an L3G4200D.  The only change was the I2C address and the WHO_AM_I value.  They'er detailed in (http://www.st.com/st-web-ui/static/active/en/resource/sales_and_marketing/presentation/product_presentation/l3gd20_l3g4200d_marketing_pres.pdf)  I also changed the fucntion names so there wouldn't be any conflict should someone want to use both at the same time?  (Two parts of an arm?  I don't know?:)

I whole heartedly support Adafruit and buy from them when I can.  They're amazing!  I would ask that you please do the same!

This unified sensor driver is for use with the L3G4200D Triple-Axis Gyro sensor.  This will work with a GY-80 IMU.  




Adafruit invests time and resources providing this open source code, 
please support Adafruit and open-source hardware by purchasing 
products from Adafruit!






## What is the Adafruit Unified Sensor Library? ##

The Adafruit Unified Sensor Library ([Adafruit_Sensor](https://github.com/adafruit/Adafruit_Sensor)) provides a common interface and data type for any supported sensor.  It defines some basic information about the sensor (sensor limits, etc.), and returns standard SI units of a specific type and scale for each supported sensor type.

It provides a simple abstraction layer between your application and the actual sensor HW, allowing you to drop in any comparable sensor with only one or two lines of code to change in your project (essentially the constructor since the functions to read sensor data and get information about the sensor are defined in the base Adafruit_Sensor class).

This is imporant useful for two reasons:

1.) You can use the data right away because it's already converted to SI units that you understand and can compare, rather than meaningless values like 0..1023.

2.) Because SI units are standardised in the sensor library, you can also do quick sanity checks when working with new sensors, or drop in any comparable sensor if you need better sensitivity or if a lower cost unit becomes available, etc. 

Light sensors will always report units in lux, gyroscopes will always report units in rad/s, etc. ... freeing you up to focus on the data, rather than digging through the datasheet to understand what the sensor's raw numbers really mean.

## About this Driver ##

Written by Kevin Townsend for Adafruit Industries.  
BSD license, all text above must be included in any redistribution

To download. click the **Download ZIP** in the right-hand column, rename the uncompressed folder Adafruit_L3G4200D_U. Check that the Adafruit_L3G4200D_U folder contains Adafruit_L3G4200D_U.cpp and Adafruit_L3G4200D_U.h

Place the Adafruit_L3G4200D_U library folder your (arduinosketchfolder)/libraries/ folder. You may need to create the libraries subfolder if its your first library. Restart the IDE.
