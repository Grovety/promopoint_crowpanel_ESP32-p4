# PromoPoint for CrowPanel ESP32-P4

PromoPoint firmware (advertising display) for **Elecrow CrowPanel Advanced ESP32-P4 panels with 1024 × 600 touch displays**.

The panel works as an advertising display and plays media from its internal flash memory or from an SD card. Content is prepared with the **Media Manager** application for Windows and uploaded to the panel over Wi-Fi, USB, or SD card.

This repository provides ready-to-use Windows packages for hardware revisions **V1.0**, **V1.1**, and **V1.2**.

## Downloads

| Package | Description |
| --- | --- |
| [MediaPlayer-for-CrowPanel-p4-v1.0-release-1.7.zip](./MediaPlayer-for-CrowPanel-p4-v1.0-release-1.7.zip) | PromoPoint firmware and the Windows flashing tool for panel **V1.0** |
| [MediaPlayer-for-CrowPanel-p4-v1.1-release-1.7.zip](./MediaPlayer-for-CrowPanel-p4-v1.1-release-1.7.zip) | PromoPoint firmware and the Windows flashing tool for panel **V1.1** |
| [MediaPlayer-for-CrowPanel-p4-v1.2-release-1.7.zip](./MediaPlayer-for-CrowPanel-p4-v1.2-release-1.7.zip) | PromoPoint firmware and the Windows flashing tool for panel **V1.2** |
| [MediaManager-for-Windows-release-1.6.zip](./MediaManager-for-Windows-release-1.6.zip) | Media Manager — the Windows application for managing the panel's media content |

## Flashing the firmware

1. Download and fully extract the firmware archive matching the panel hardware revision.
2. Connect the panel's **UART0 USB-C port** to a Windows computer using a data-capable USB cable.
3. Open the extracted folder.
4. Run the `MediaPlayer-for-CrowPanel-...-Flasher.exe` application from the extracted folder.
5. Select the panel's COM port. Click **Refresh** if the port is not listed.
6. Make sure **Clean install (erase entire flash)** is enabled.
7. Click **Flash panel**.
8. Do not disconnect the panel while flashing.
9. Wait for the **Firmware installed successfully** message.

The panel restarts automatically after flashing.

## Installing Media Manager

1. Download and fully extract `MediaManager-for-Windows-release-1.6.zip`.
2. Run `MediaManagerForCrowPanel-Setup-win-x64-1.6.exe`.
3. Follow the installer instructions.

## Troubleshooting

If the panel is not detected, reconnect it through UART0, close any application using the COM port, and click **Refresh**.

If the COM port still does not appear, install the [CH341 USB serial driver](https://www.wch-ic.com/downloads/CH341SER_ZIP.html), reconnect the panel, and click **Refresh** again.
