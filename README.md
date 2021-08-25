



# How-to-program-ESP8266-nodeMCU-with-Arduino-IDE-LED-Blink

![image](https://user-images.githubusercontent.com/19898602/130723279-c5718b37-814b-44a0-be4d-61a9983007e5.png)


In this post we”ll learn how easily we can program our ESP8266 NodeMCU with Arduino IDE we will upload a simple sketch of LED blink to ESP8266 board

It is very simple to load code to ESP8266 using Arduino IDE same as we are doing for Arduino boards but first we need to do a simple step of adding ESP8266 board in Arduino IDE.


## Adding ESP8266 Board in arduino IDE


First of all off-course we need to download Arduino IDE to upload codes to if you already installed it in your computer you can move ahead.
or you can download it from here.

First install the IDE on you PC and open the IDE, now go to
FILE > PREFERENCES

![image](https://user-images.githubusercontent.com/19898602/130723328-8c8e703a-386f-468f-8ce6-d54b50a61d91.png)



Now go to the “Additional boards manager URLs”
and past this link there :
http://arduino.esp8266.com/stable/package_esp8266com_index.json
and click on OK.



![image](https://user-images.githubusercontent.com/19898602/130723385-b6f547d7-7a0a-4bc8-b45d-d44b9e02b5db.png)


Now go to : Tools > Board > Board manager


![image](https://user-images.githubusercontent.com/19898602/130723405-ea114fa3-33fd-46a0-9719-3bc1018c0e41.png)



Now search for “ESP8266” and click on “Install” and wait for some time to install board to arduino IDE



![image](https://user-images.githubusercontent.com/19898602/130723421-35356ef6-a62b-43b4-a4f3-78bfbb5f7e19.png)


In this way we successfully added ESP8266 board to our arduino IDE to verify you can go to : Tools > Boards and scroll to the bottom of list you will see whole list of new boards are live to be use.

![image](https://user-images.githubusercontent.com/19898602/130723441-67ebd716-fa21-445e-8367-8d7157f6309a.png)


## Uploading code to ESP8266 NODEMCU

Simply connect the LED with ESP8266 board as shown in image
connect positive leg of LED TO D1 pin
and negative leg of LED to GND pin

![image](https://user-images.githubusercontent.com/19898602/130723466-6cf0dcd6-a30e-41a2-8826-1edd72f1a93d.png)


Simply connect the ESP8266 board to PC using Micro USB cable
Open the arduino and select the board which is “NodeMCU 1.0(ESP-12E Module)”



![image](https://user-images.githubusercontent.com/19898602/130723492-ca5dfbfa-95f5-405e-b9d6-b049349d3f97.png)


Select the proper port from here at which you ESP8266 nodeMCU is connected


![image](https://user-images.githubusercontent.com/19898602/130723517-3bd3a69e-bca9-44fe-b8a7-15b6f8a29321.png)


Now upload the following code to ESP8266 simply by clicking on upload button.
after uploading the you will see LED start to blink with 1 second delay.


```cpp
int LED = 5; // Assign LED pin i.e: D1 on NodeMCU

void setup() {

// initialize GPIO 5 as an output

pinMode(LED, OUTPUT);

}

// the loop function runs over and over again forever

void loop() {

digitalWrite(LED, HIGH); // turn the LED on
delay(1000); // wait for a second
digitalWrite(LED, LOW); // turn the LED off
delay(1000); // wait for a second

}
```

## ESP8266, TUTORIALS

How to program ESP8266 nodeMCU with Arduino IDE | LED Blink
Posted by sandeep on May 13, 2020
Esp8266-nodeMCU-programming-with-Arduino-IDE

 

In this post we”ll learn how easily we can program our ESP8266 NodeMCU with Arduino IDE we will upload a simple sketch of LED blink to ESP8266 board

It is very simple to load code to ESP8266 using Arduino IDE same as we are doing for Arduino boards but first we need to do a simple step of adding ESP8266 board in Arduino IDE.

Adding ESP8266 Board in arduino IDE
First of all off-course we need to download Arduino IDE to upload codes to if you already installed it in your computer you can move ahead.
or you can download it from here.

First install the IDE on you PC and open the IDE, now go to
FILE > PREFERENCES

Esp8266 nodeMCU Arduino IDE
Esp8266 nodeMCU Arduino IDE


Now go to the “Additional boards manager URLs”
and past this link there :
http://arduino.esp8266.com/stable/package_esp8266com_index.json
and click on OK.

Esp8266 nodeMCU Arduino IDE
Esp8266 nodeMCU Arduino IDE

 


Now go to : Tools > Board > Board manager

Esp8266 nodeMCU Arduino IDE
Esp8266 nodeMCU Arduino IDE


Now search for “ESP8266” and click on “Install” and wait for some time to install board to arduino IDE




In this way we successfully added ESP8266 board to our arduino IDE to verify you can go to : Tools > Boards and scroll to the bottom of list you will see whole list of new boards are live to be use.



 
Uploading code to ESP8266 NODEMCU
Simply connect the LED with ESP8266 board as shown in image
connect positive leg of LED TO D1 pin
and negative leg of LED to GND pin

ESP8266 nodeMCU LED Blink
ESP8266 LED blink
Simply connect the ESP8266 board to PC using Micro USB cable
Open the arduino and select the board which is “NodeMCU 1.0(ESP-12E Module)”


Select the proper port from here at which you ESP8266 nodeMCU is connected


Now upload the following code to ESP8266 simply by clicking on upload button.
after uploading the you will see LED start to blink with 1 second delay.

int LED = 5; // Assign LED pin i.e: D1 on NodeMCU
void setup() {
// initialize GPIO 5 as an output
pinMode(LED, OUTPUT);
}
// the loop function runs over and over again forever
void loop() {
digitalWrite(LED, HIGH); // turn the LED on
delay(1000); // wait for a second
digitalWrite(LED, LOW); // turn the LED off
delay(1000); // wait for a second
}
ESP8266 GPIO PINs Details in reference of ARDUINO IDE


![image](https://user-images.githubusercontent.com/19898602/130723665-1060329f-25ae-4510-a727-cb3962977c0e.png)


![image](https://user-images.githubusercontent.com/19898602/130723671-49e7f75d-26ce-4960-860f-135bc17e87f5.png)





https://user-images.githubusercontent.com/19898602/130723790-8a1afc2f-16ac-4d14-b86e-7c31e72e5b53.mp4




At last I would like to tell you something about PCB 

Yes PCB are the heart of the electronics based project usually we hesitate to try custom PCB and opt to homemade solutions

like breadboard or Zero PCB earlier I also was in the same boat, I hesitate to try custom PCB my belief was they are much expensive.

but then I came to know about [JLCPCB.com](https://jlcpcb.com/IAT) and I was totally surprised how low price PCB's are they offering 

there PCB quality is top to the mark now I always go with PCB for my project and [JLCPCB.com](https://jlcpcb.com/IAT) is my trusted 

PCB manufacturer, you can also try there PCB service for more details you can visit their website [JLCPCB.com](https://jlcpcb.com/IAT)



![MVI_0001 00_04_10_14 Still001](https://user-images.githubusercontent.com/19898602/130724059-6487bb30-e6cc-439f-a38a-a58052126d7f.jpg)
![MVI_0035 00_03_44_09 Still007](https://user-images.githubusercontent.com/19898602/130724080-99281955-cadb-4679-97f1-456c8223d777.jpg)
![MVI_5077 00_01_32_03 Still004](https://user-images.githubusercontent.com/19898602/130724116-648354c0-f1b5-4d8c-850c-3b6aff622e67.jpg)






