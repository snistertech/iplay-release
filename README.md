# iPlay Kiosk

A simple installation and usage guide.

## What It Does

- Runs a kiosk portal
- Supports app whitelist control
- Uses coin pulse input from ESP32
- Supports Device Owner setup using QR provisioning
- Includes admin panel settings

## Android App Installation

- Download the published Android APK.
- Install it on the device.

## ESP32 Installation Guide

- Download the published firmware file: `iplay-esp32.bin`.
- Flash `iplay-esp32.bin` to your ESP32 using your preferred flash tool.
- Restart ESP32 after flashing.

## Device Owner QR Provisioning

1. Prepare your provisioning QR JSON with the APK URL and checksum.
2. Generate a QR image from the provisioning JSON.
3. Factory reset the Android device.
4. On setup wizard, scan the provisioning QR code.
5. Complete setup and connect to Wi-Fi when asked.

## App Update Flow

- Keep the same package name and signing key for updates.
- Install the newer APK version directly on provisioned devices.
- For new devices, use an updated provisioning QR that matches the current APK checksum.

## Troubleshooting

- Provisioning fails: verify the provisioning QR data and checksum match the current APK.
- QR works but install fails: confirm APK is not HTML/redirect page.
- Bluetooth offline: ensure phone Bluetooth is ON and permissions are granted.
