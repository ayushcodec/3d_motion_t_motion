# 3D Motion T-Motion (MPU6050 + SSD1306 + MKR1010)
 This project uses the MPU6050 motion sensor, Mini OLED SSD1306, and Arduino MKR1010 to render 3D objects on the OLED display and rotate them using real-time motion from the MPU6050.

The code can be easily converted for any microcontroller (ESP32, ESP8266, Arduino Nano, UNO, etc.) using ChatGPT.

🚀 Features

✔ Real-time 3D motion rendering
✔ MPU6050 gyro + accelerometer tracking
✔ Works with MKR1010 (default)
✔ Portable code, easy to adapt to other boards
✔ Only 3 libraries required

📦 Step 1: Install Required Libraries

#include <Adafruit_GFX.h>
#include <Adafruit_SSD1306.h>
#include <MPU6050.h>
You can install them from:

Arduino IDE → Tools → Manage Libraries → Search → Install

**🧩 Step 2: Install MKR1010 Board Package**

Open Arduino IDE

Go to
Tools → Board → Boards Manager

Search:
“Arduino SAMD Boards (32-bit ARM Cortex-M0+)”

Install it
(This adds support for MKR1010)

**🔌 Step 3: Make the Connections**

Open the connections folder and follow the wiring diagram.
Typical connections:
MPU6050 → MKR1010
SDA → SDA
SCL → SCL
VCC → 3.3V
GND → GND

SSD1306 OLED → MKR1010
SDA → SDA
SCL → SCL
VCC → 3.3V
GND → GND

**💻 Step 4: Upload Code**
Open the code folder
In Arduino IDE set:
Tools → Board → Arduino MKR WiFi 1010
Select Port
Click Upload
Once uploaded, the OLED will display a 3D shape rotating according to MPU6050 movement.

**Using Other Microcontrollers?
**
This project works with many boards:
ESP32
ESP8266
Arduino Nano
Arduino UNO
AVR / ARM boards
You can ask ChatGPT to automatically convert the code for your board.
