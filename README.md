# AI Teacher ESP Shield v2

## Download for uploading the same code

**[Download the small flash-only ZIP](https://github.com/Prem-things/ai-teacher-/releases/latest/download/AI_Teacher_ESP_Shield_V2_Flash_Only.zip)**

This is the package to share with a friend who needs to upload the supplied firmware with its original pins and audio. No Python, Arduino IDE, compiler, or library installation is required.

1. Extract the **entire ZIP**.
2. Connect a classic ESP32 DevKit by USB.
3. Double-click **AI Teacher ESP Shield v2 Flasher.exe**.
4. Select the board's COM port and click **Flash ESP32 — firmware + audio**.

The app uploads the firmware and audio/logo filesystem together. Keep the included folders beside the EXE. If no COM port appears, use **USB driver setup**; the offline drivers are included, and Windows may request administrator approval. Close Arduino Serial Monitor before flashing. If necessary, use 115200 baud and hold BOOT until the upload connects.

## Editable version

**[Download the larger editable flasher ZIP](https://github.com/Prem-things/ai-teacher-/releases/latest/download/AI_Teacher_ESP_Shield_V2_Flasher.zip)** only if you want to change pins or rebuild the code. That package includes the complete offline ESP32 compiler and libraries, so it is much larger.

## Preserved firmware

Firmware: `ai_teacher_esp_shield_v2.ino`, supplied by the owner. Original WiFi/API settings are retained as requested. The original MP3 playback implementation, all 41 MP3 clips, the logo, display setup, and startup behavior are preserved. Checksums are included in the packages.

| Signal | Default GPIO |
|---|---:|
| TFT CS / DC / reset | 12 / 33 / 32 |
| TFT MOSI / clock | 23 / 18 |
| TFT MISO / backlight | unused / unused |
| Next / Select / Home buttons | 4 / 5 / 19 |
| Speaker DAC | 25 |
| Initial startup HIGH pin | 19 |

Target: **classic ESP32, 4MB flash**. ESP32-S3/C3 boards are not supported by this firmware. Existing saved WiFi settings are retained; no full-chip erase is performed. The existing WiFi setup portal remains available when the saved/default network is unavailable.
