### Project 14 LM35 Linear Temperature Sensor

![](media/wps7-1764318334863-1.png)

**1.Introduction**

LM35 Linear Temperature Sensor is based on semiconductor LM35 temperature sensor. It can be used to detect ambient air temperature. This sensor offers a functional range among 0 degree Celsius to 100 degree Celsius. Sensitivity is 10mV per degree Celsius. The output voltage is proportional to the temperature.

This sensor is commonly used as a temperature measurement sensor. It includes thermocouples, platinum resistance, and thermal resistance and temperature semiconductor chips. The chip is commonly used in high temperature measurement thermocouples. Platinum resistance temperature sensor is used in the measurement of 800 degrees Celsius, while the thermal resistance and semiconductor temperature sensor is suitable for measuring the temperature of 100-200 degrees or below, in which the application of a simple semiconductor temperature sensor is good in linearity and high in sensitivity. The LM35 linear temperature sensor and sensor-specific Arduino shield can be easily combined.

**2.Specification**

- Based on the semiconductor LM35 temperature sensor
- Can be used to detect ambient air temperature
- Sensitivity: 10mV per degree Celcius
- Functional range: 0 degree Celsius to 100 degree Celsius
- Size: 30*20mm
- Weight: 3g

**3.Connection Diagram**

![](media/wps8-1764318411484-3.jpg)

**4.Sample Code**

```c
void setup()
{
    Serial.begin(9600);//Set Baud Rate to 9600 bps
}

void loop()
{  
    int val;
    int dat;
    val=analogRead(0);//Connect LM35 on Analog 0
    dat=(500 * val) /1024;;
    Serial.print("Temp:"); //Display the temperature on Serial monitor
    Serial.print(dat);
    Serial.println("C");
    delay(500);
}
```

