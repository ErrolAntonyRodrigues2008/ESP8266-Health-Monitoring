Health monitoring is the major problem in today’s world. Due to lack of proper health monitoring, patient suffer from serious health issues. There are lots of IoT devices now days to monitor the health of patient over internet. Health experts are also taking advantage of these smart devices to keep an eye on their patients. With tons of new healthcare technology start-ups, IoT is rapidly revolutionizing the healthcare industry.

Items required:
Arduino Uno 
ESP8266 Wi-Fi module
LM35 temperature sensor
Pulse rate sensor
Push button
10k Resistor
Male-female wires
Breadboard

Below are the connections:

Signal pin of pulse sensor -> A0 of arduino
Vcc pin of pulse sensor -> 5V of arduino
GND pin of pulse sensor -> GND of arduino
Vout of LM35 -> A1 of Arduino
Tx of ESP8266 -> pin 10 of arduino
Rx of ESP8266 -> pin 11 of arduino
CH_PD and Vcc of ESP8266 -> 3.3 V of arduino
GND of ESP8266 -> GND of arduino
Push button ->  digital pin 8 of arduino

ThingSpeak Configuration

Step 1:- First of all, user needs to Create a Account on ThingSpeak.com, then Sign In and click on Get Started.
![image](https://github.com/user-attachments/assets/72259943-8c1e-4eff-89f8-1650bd4dfb12)

Step 2:-  Now go to the ‘Channels’ menu and click on New Channel option on the same page for further process.
![image](https://github.com/user-attachments/assets/71e268ae-b7d0-42a2-8414-a262aa37ec34)

Step 3:- Now you will see a form for creating the channel, fill in the Name and Description as per your choice. Then fill ‘Pulse Rate’, ‘Temperature’ and ‘Panic’ in Field 1, Field 2 and Field 3 labels, tick the checkboxes for the Fields. Also tick the check box for ‘Make Public’ option below in the form and finally Save the Channel. Now your new channel has been created.
![image](https://github.com/user-attachments/assets/9d943f5c-7503-4145-a6ad-d8464e95e704)

Step 4:- You will see three charts as shown below. Note the Write API key, we will use this key in our code.
![image](https://github.com/user-attachments/assets/b148b2d7-5575-411a-a882-9562e4092420)

Step 5:- Now, we will use ThingHTTP app of the server to trigger the IFTTT applet for data entry to Google sheets and send email/sms. ThingHTTP enables communication among devices, websites, and web services without having to implement the protocol on the device level. You can specify actions in ThingHTTP, which you want to trigger using other ThingSpeak apps such as React.

To make New ThingHTTP, we will need URL for triggering which we will get from IFTTT.
![image](https://github.com/user-attachments/assets/ba2c5800-7e49-4ba3-b0e7-3455748127dd)









