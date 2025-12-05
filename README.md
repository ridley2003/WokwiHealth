# WokwiHealth


WokwiHealth is a simulated patient-vitals system. It uses an ESP32 running FreeRTOS inside of the Wokwi environment, using the Arduino coding style. The real-time modality of this project is important. When patients are having an emergency, swift response time can be the difference between life and death.

There are two LEDs. The green LED symbolizes the "system heartbeat" - an indicator that the system is online and functioning properly. The red LED shines for a short period when an emergency triggers. There are 3 ways to cause this. The primary way is that the system will detect when the patient's heartrate has reached a dangerous level. The patient is also able to press a small yellow button near their bed. If a healthcare provider monitors the vitals from a distance, they can also trigger an emergency by using an HTTP server, which contains its own emergency button along with the current vitals. In any case, it will have the effect of rushing nurses over to the patient's room so that they can assist. 

Finally, the Wokwi Logic Analyzer, connected to the simulated board, is able to export a timeline which can be viewed in the PulseView application. Here, providers can see exactly when emergencies were triggered, including when the sensor received new values and when the pushbutton was pressed.

You can see a simple demonstration of WokwiHealth here (click the image):

[![](https://img.youtube.com/vi/IjPqxBrq4KE/0.jpg)](https://youtu.be/IjPqxBrq4KE)
