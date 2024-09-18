# Gridlights Demo App

First demo app for the 8x8 LED square.

## SOP for Configuring LED Light with ESP32

### Step 1: Install WLED on the ESP32 Chip
1. Connect the ESP32 chip (connected to the WiFi device) to your computer.
2. Open your browser and navigate to the [WLED Install Page](https://install.wled.me/).
3. Install the latest **non-beta** version of WLED.
4. Wait for the installation to complete.
5. When prompted to configure WiFi, **skip** this step.

### Step 2: Flash the Other ESP32 Chip
1. Connect the second ESP32 chip to your computer.
2. Open a terminal or command prompt.
3. Run the following command to erase the flash on the ESP32 (ensure you update the port if necessary):
   ```
   esptool.py --chip esp32 --port /dev/tty.SLAB_USBtoUART erase_flash
    ```
4. Wait for the process to complete.
### Step 3: Upload Code to the ESP32
1. Download the code from GitHub:
```
git clone https://github.com/mjgriffin1113/gridlights-demo-app
```
2. Make sure Python is installed on your computer.
3. Run the Python script to upload the code to the ESP32:
```
python upload_to_esp32.py
```
4. Access the LED Controller
1. Once the upload is complete, navigate to 4.3.2.2 in your browser.
2. Start using the app to control the LED light!