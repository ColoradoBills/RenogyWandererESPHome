# RenogyWanderESPHome
HACS Integration to allow you to track data from your Renogy Wander Solar Controller via ESPHome in Home Assistant

*** Please ensure you are skilled to work around electrical components that could cause serious injuries if you are not safe. Solar panels can produce curret that can cause serious injuries, including death. Be safe ***

Parts Required:
  1) D1 Mini (or other ESP32/ESP8266 board) - I used a D1 Mini 8266 [https://amzn.to/3ERUsoe]
  2) Renogy Wanderer Solar Controller [https://amzn.to/3CJEbBr]
  3) TTL to RS32 Module [https://amzn.to/3EH5nkN]
  4) RJ11 Connector - This is to allow you to connect into th Renogy Wanderer Solar Controller [https://amzn.to/3CYWGSj]
  5) ** You can buy a small RJ11 patch cable and cut one end off if you don't have crimpers [https://amzn.to/3CYbKzF]
  6) RJ11/RJ45 Crimp Tool [https://amzn.to/3X6eulv]
  7) Waterproof Box for Outside [https://amzn.to/411QnoX] - I bought this in 2000 and it is still going great today.

* I used some extra CAT5 cable laying around as the patch cable for this project. You don't need much *

Here is the pinout for the RJ11 connector - Remember the TX of the RJ11 goes the RX of th TTL to RS232 Module - You will have issues if you go TX to TX and RX to RX. 

![RJ11 Pinout](https://github.com/ColoradoBills/RenogyWandererESPHome/blob/d81924c0b96decb94ac35d26a2b136393f8d8cc5/images/CE45E8AB-9ED6-446E-A3B0-C6F7A7CD1B8C.jpeg)

Connect the RJ11 patch cable to the TTL to RS232 module. Connect the Module to your ESP board [follow the pins in th YAML code if you are using a D1 Mini 8266].

Add your ESP board to Home Assistant via ESPHome addon. 
Copy the YAML from this Repo to the YAML of your new ESP Home Device in Home Assistant
*** Don't Forget to go to SETTINGS -> INTEGRATIONS to add your new ESPHome device. If you do not do this, you will not see any of the new sensors. 

You can now add these sensors to your Home Assistant Energy dashboard, create automations, or so many other things. 
