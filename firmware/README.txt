================================================================================
  YETI OFFICIAL FIRMWARE RELEASES (OTA READY)
================================================================================

This directory contains the latest ready-to-flash compiled firmware binaries for
the Yeti Desktop Robot Companion.

FILES:
--------------------------------------------------------------------------------
1. YETI_ESP32_CAM_LATEST.bin
   - Hardware: AI-Thinker ESP32-CAM (4MB Flash, dual 1.9MB OTA slots)
   - Scheme:   min_spiffs
   - Size:     ~1.2 MB
   - Use for:  Wireless Bluetooth BLE OTA updates or USB flashing on ESP32-CAM.

2. YETI_ESP32_C3_LATEST.bin
   - Hardware: ESP32-C3 SuperMini (4MB Flash, dual 1.25MB OTA slots)
   - Scheme:   default
   - Size:     ~810 KB
   - Use for:  Wireless Bluetooth BLE OTA updates or USB flashing on ESP32-C3.

HOW TO FLASH WIRELESSLY OVER BLE (SMARTWATCH STYLE):
--------------------------------------------------------------------------------
1. Open the laptop controller: launch_controller.bat
2. Click "Connect BLE" to pair with your Yeti (YETI-XXXX).
3. Switch to the "⚡ Firmware OTA Update" tab.
4. Click "Load Current ESP32-CAM Binary" (or "Load Current ESP32-C3 Binary").
5. Click "⚡ Start Wireless BLE Firmware Update".
6. The robot detents servos, displays the live OTA progress bar, and reboots!

AUTOMATIC BUILD PIPELINE:
--------------------------------------------------------------------------------
Running 'build_cam.bat' or 'build_c3.bat' automatically recompiles the sketch
and copies the verified binary directly into this folder as the LATEST release!
================================================================================
