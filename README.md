# Arduino monitor water level

This project will check water level in tank with HC-SR04 ultrasonic sensor, show in 0.96 inch OLED Display and send distance to firebase realtime database for React dash board in next project.

## Arduino Library use
1. Arduino core for ESP8266 WiFi chip: https://github.com/esp8266/Arduino
2. Firebase Realtime Database Arduino Library for ESP8266 and RP2040 Pico: https://github.com/mobizt/Firebase-ESP8266
3. Adafruit_SSD1306: https://github.com/adafruit/Adafruit_SSD1306

## Need to change code before use
```
#define FIREBASE_HOST "Firebase database URL"
#define FIREBASE_AUTH "Database Secrets"
```
```
#define WIFI_SSID "Wifi Username"
#define WIFI_PASSWORD "Wifi Password"
```
```
IPAddress ip(192, 168, 0, 100); //Wifi IPAddress
```
```
int maxDist = 1000; // Tank Height or full water level you need in millimeters
```

## Result in firebase realtime database
<img alt="Firebased realtime database" src="https://i.ibb.co/mTXLQSX/Screenshot-2023-03-25-174941.png">

## Diagram

## HC-SR04 Ultrasonic Sensor

## 0.96 inch OLED Display
