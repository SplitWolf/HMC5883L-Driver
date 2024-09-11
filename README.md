# HM5883L Driver

Driver for the HM5883L compass module, for an arduino based microcontroller

# Includes

Add the correct wire library file for your board, and <stdint.h>

# Initilization

Initilize the driver by calling the constructor with the SDA and SCL pins and then calling the begin method during setup

```
driver = HMC5883L::HMC5883L(sCL_PIN,sDA_PIN)
driver.begin()
```

# Reading Data

The `isDataReady()` method can be called to check the register on the device for when the data is ready to be read then `readData()` can be used to read the data

# Settings

The gain, mode, data rate, and sample count can be set using the appropriate methods

# Self Test

The `selfTest()` method can be used to run the device self test and returns the data