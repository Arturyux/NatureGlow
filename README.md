# **NatureGlow**  
## **Bridging Outdoor Light to Indoors Smart Bulb Adaptation**  

**Author:** Artur Burlakin  
**Student code:** ab226ij  

---

### 1. **About the Project**

- **NatureGlow**: A unique sensor system designed to harmonize indoor lights with the ambient colors of the outside environment. Beyond this, it gauges the outside light, temperature, and humidity – predicting forthcoming weather patterns, promoting better weather understanding, and nurturing a more naturalistic indoor ambiance.

- **Project Duration**: There was a problem as I forgot my materials at the university during summer vaccation and traveled away, which delayed my progress. Nevertheless, I wrapped up the project within a week.

---

### 2. **Objective**

- **2.1 Motivation Behind the Project**: My inherent passion for nature coupled with a curiosity to explore the correlation between indoor comfort and external conditions prompted this venture. The central idea was to discern if indoor illumination can be tailored to emulate the external light, lending a more natural feel.

- **2.2 Significance**: NatureGlow endeavors to bring the great outdoors into our living spaces by mirroring the external light inside. This not only augments the intrinsic comfort but potentially predicts weather shifts by observing variations in external light, temperature, and humidity.

- **2.3 Expected Outcomes**: By mapping the interrelations between external light, temperature, and humidity, I posit that we can get a glimpse into forthcoming weather changes, prepping us for the unpredictable – be it rain, sunshine, or a sudden transition.

---

### 3. **Materials Used**

- **Adafruit ESP32-S3 TFT Feather**: The brain behind the operations, equipped with 4MB Flash, 2MB capacity, and STEMMA connectivity. [Product Link](https://www.adafruit.com/product/5483) 


- **Adafruit Sensirion SHT40 Sensor**: An instrument for gauging ambient temperature and humidity, delivering real-time insights. [Product Link](https://www.adafruit.com/product/4885) 


- **Adafruit APDS9960 Sensor**: A multifunctional sensor adept in estimating distances, evaluating light intensity, recognizing colors, and detecting hand gestures. [Product Link](https://www.adafruit.com/product/3595) 

- **Yeelight Bulb W3(MultiColor)**: RGB bulb to customize colors. [Product Link](https://www.proshop.se/Smarta-Hem/Yeelight-LED-Smart-Bulb-W3-Multicolor/2936381?utm_source=google&utm_medium=cpc&utm_campaign=searchengine&gclid=CjwKCAjwoqGnBhAcEiwAwK-OkSfifzeAruSrDAopcelVbhz3p0wrUt6ZxShWfLgBoh1u7oyTDofUKBoCm5gQAvD_BwE) 


- **USB-C Cable**: Vital for powering and establishing connectivity with the main board.

- **STEMMA Cable Connectors**: Facilitate smooth connections between the board and sensors, bypassing the need for soldering.



---

### 4. **Computer Configuration**

- **Platform**: I leveraged **Visual Studio Code (VSCode)**, a multifaceted editor compatible with a broad spectrum of programming languages, including Python.

    - **4.1 CircuitPython Firmware Installation**:
        1. Connected the Adafruit ESP32-S3 TFT Feather via USB-C.
        2. Performed a hard reset by pressing the Boot button for 5 seconds, followed by the Reset button.
        3. Procured the latest CircuitPython firmware for Feather ESP32-S3 TFT PSRAM from the official website.
        4. Utilized ESP Web Flasher, connecting to the device 115200 port, and uploading the firmware.

    - **4.2 Setting up VSCode**:
        1. Procured VSCode from its official portal.
        2. Made use of the HomeBrew package already installed on my computer.
        3. Terminal Command: `brew install python3`
        4. Installed CircuitPython libraries: `pip3 install adafruit-circuitpython-bundle`
        5. Integrated required libraries (adafruit_sht4x.mpy & adafruit_apds9960.mpy) by dragging them into the 'lib' folder.

    - **4.3 Code Deployment**:
        1. Authored the code within VSCode.
        2. Post finalization, saved the script as `code.py`.
        3. Directly transported the `code.py` file to the root of the CIRCUITPY drive. CircuitPython then autonomously detected and ran the code.

---

### 5. **Data Transmission & Connectivity**

- **5.1 Transmission Frequency**: Sensor data acquisition and dispatch happen every 5 minutes – striking a balance between real-time updates and energy conservation.

- **5.2 Wireless Protocols**: WiFi is the chosen medium, given its balance of transmission speed and range, especially suited for indoors settings.

- **5.3 Transport Protocols**: Data is transmitted to our database via the HTTP protocol. This is done by forwarding the sensor data as requests, which subsequently interacts with the ThingSpeak Cloud database.

---

### 6. **Data Presentation**

- **6.1 Database Update Frequency**: Data entries are updated every 5 minutes in the database.

- **6.2 Database Selection Rationale**: I transitioned to ThingSpeak, a cloud-based database, for the project's data storage needs. 

    **About ThingSpeak**:
    ThingSpeak is an IoT analytics platform service that allows you to aggregate, visualize, and analyze live data streams in the cloud. It provides real-time data collection from embedded devices and then uses MATLAB analytics to delve into the data. The platform is popular for its ease of use, integration capabilities, and robust API, making it a prime choice for IoT projects. 


---

### 7.1 **Project Finalization**

- **7.1 Future Improvements**: I envision incorporating a battery to eliminate the need for a USB-C cable, a feature already anticipated in the design. One of the sensors can detect motion, enabling user interaction even from across a window. A simple hand gesture (e.g., waving down) could trigger an instant data dispatch, while another gesture (e.g., waving up) might reset the entire system.
### 7.2 **Pictures**
![](https://hackmd.io/_uploads/B1Y1xsLpn.jpg)
![](https://hackmd.io/_uploads/H1Yklo862.jpg)
![](https://hackmd.io/_uploads/H19ygsLph.jpg)
![](https://hackmd.io/_uploads/SkqJgsIpn.jpg)



