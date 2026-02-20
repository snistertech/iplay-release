# iPlay Kiosk

A simple installation and usage guide.

Admin password: admin1234

## What It Does

- Runs a kiosk portal
- Supports app whitelist control
- Uses coin pulse input from ESP32
- Supports Device Owner setup using QR
- Includes admin panel settings
- Android 8.0 to 15 support.

## ESP32 Installation Guide

- Download the published firmware file: `iplay-esp32.bin`.
- Flash `iplay-esp32.bin` to your ESP32 using your preferred flash tool.
- Restart ESP32 after flashing.

## Device Owner 

2. Download the Qr image.
3. Factory reset the Android device.
4. On setup wizard, tap 6 to 10 times to show  QR scan and scan the downloaded qr image.
5. Complete setup and connect to Wi-Fi when asked.

## App Update Flow

- Install the newer APK version directly.

## Troubleshooting

- Provisioning fails: verify the provisioning QR code or contact the owner.
- QR works but install fails: confirm APK is not HTML/redirect page.
- Bluetooth offline: ensure phone Bluetooth is ON and permissions are granted.
