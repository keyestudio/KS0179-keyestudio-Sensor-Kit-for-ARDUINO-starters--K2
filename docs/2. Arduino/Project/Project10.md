### Project 10 White LED Module

![](media/wps1.png)

**1.Introduction** 

This is a special LED module. When you connect it to ARDUINO development board, after program, it can emit beautiful light. Of course, you can also control it using PWM. It will be like fireflies at night. Isn’t cool? We can also combine it with other sensors to do various interesting interactive experiments. 

**2.Specification** 

- Module type: digital
- Working voltage: 5v
- Distance between pins: 2.54mm
- Size: 30*20mm
- Weight: 3g

**3.Connection Diagram**

![](media/wps2-1764292655808-2.jpg)

**4.Sample Code**

```c
int led = 3;

void setup()
{
  pinMode(led, OUTPUT);     //Set Pin3 as output
}

void loop()
{
   digitalWrite(led, HIGH);   //Turn on led
   delay(2000);
   digitalWrite(led, LOW);    //Turn off led
   delay(2000);
}
```

