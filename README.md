A repository for stable versions of sensor documentation and instructions.

Each stable sensor manual will have it's own directory in this repository. Each directory has subdirectories of "firmware" and "hardware" which include descriptions of how to program and how to build the entire sensor unit. Below are descriptions:

WL_SE - Water Level Standard Edition. This is a LoRaWAN enabled distance sensor built on a Heltec HTCC-AB02 MCU using a Maxbotix MB7389 (or MB7388) ultrasonic sensor. It is solar powered.

WL_SE_USTemp - Water Level Standard Edition + Ultrasonic Temp. This is a LoRaWAN enabled distance sensor as above, except it also is enabled to read the internal thermistor built into the maxbotix ultrasonic sensor. This can be useful if you want to use the ultrasonic sensor to calculate air temperature when flooding is not occurring.