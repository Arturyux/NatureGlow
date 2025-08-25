# NatureGlow  
**Bridging Outdoor Light to Indoors – Smart Bulb Adaptation**

**Full name:** Artur Burlakin  
**Student code:** ab226ij  

---

## 1. About the Project: NatureGlow
NatureGlow is a special sensor system that matches your indoor lights to the outside colors.  
But it does more than that: it also checks the outside light, warmth, and wetness to help guess the coming weather.  
This helps us understand the weather better, all while making our indoor spaces feel more natural.  

---

## 2. Objective
**Why I Chose the Project:**  
I love nature and I've always been curious about the link between indoor comfort and outdoor conditions.  
Plus, I wanted to see if indoor lights could feel more natural by matching them with the outdoor light.  

**What Purpose Does It Serve:**  
NatureGlow helps make our indoor spaces feel like the outdoors.  
It adjusts indoor lighting to be like the light outside, making being inside feel more natural and comfortable.  
Also, by studying how outdoor light, temperature, and humidity change, it might help guess the weather.  

**What Insights I Think It Will Give:**  
By looking at how light, warmth, and wetness outside are connected, I think we can get a better idea about the coming weather.  
This can make us more ready for rain, sunshine, or any changes.  

---

## 3. Materials
- **1x Adafruit ESP32-S3 TFT Feather**  
  Main board that controls everything. It has 4MB Flash and 2MB capacity and connects using STEMMA.  
- **1x Adafruit Sensirion SHT40 Sensor**  
  Measures temperature and humidity. Provides real-time data on the environment.  
- **1x Adafruit APDS9960 Sensor**  
  Multipurpose sensor: detects proximity, measures light levels, senses colors and hand movements.  
- **1x USB-C Cable**  
  Used to connect and power the main board.  
- **2x STEMMA Cable Connectors**  
  Easy connection between board and sensors without soldering.  

---

## 4. Computer Setup
I used **Visual Studio Code (VSCode)**, a versatile editor that supports many programming languages, including Python.  

### 4.1 Installing CircuitPython Firmware
1. Connected the **Adafruit ESP32-S3 TFT Feather** to my computer using the USB-C cable.  
2. Held the **Boot** button for about 5 seconds, then pressed **Reset** at the same time → hard reset.  
3. Downloaded the latest CircuitPython firmware for the Feather ESP32-S3 TFT PSRAM from the CircuitPython website.  
4. Used **ESP Web Flasher**, connected device at 115200 port, and uploaded the firmware.  

### 4.2 Setting Up VSCode
1. Installed VSCode from its official website.  
2. Installed **HomeBrew** package manager.  
3. In terminal, ran:  
  ```bash
   brew install python3
  ```

   ![Loading](https://github.com/Arturyux/NatureGlow/blob/main/images/IMG_9720.jpg)

   ![Loading](ttps://github.com/Arturyux/NatureGlow/blob/main/images/IMG_9721.jpg)

   ![Loading](https://github.com/Arturyux/NatureGlow/blob/main/images/IMG_9722.jpg)