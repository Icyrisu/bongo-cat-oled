# 🐾 Bongo Cat OLED Animation with Arduino

This repository contains an Arduino sketch that displays an animated **Bongo Cat** on a **128x64 OLED** screen using the **SSD1306 driver** and **Adafruit libraries**.

## 📦 Features

- Cute animated Bongo Cat on an OLED screen
- Uses frame-based animation with custom bitmap images
- Designed for SSD1306 128x64 I2C OLED displays
- Fully compatible with Arduino Uno, Nano, Mega, and ESP boards

## 🧰 Requirements

Make sure you have the following libraries installed in your Arduino IDE:

- [`Adafruit_SSD1306`](https://github.com/adafruit/Adafruit_SSD1306)
- [`Adafruit_GFX`](https://github.com/adafruit/Adafruit-GFX-Library)
- `Wire` (usually included with the Arduino IDE)

You can install them via the Library Manager (`Sketch > Include Library > Manage Libraries...`).

## 🔌 Wiring

| OLED Pin | Arduino Pin |
|----------|-------------|
| VCC      | 5V          |
| GND      | GND         |
| SDA      | A4 (or D21 on ESP32) |
| SCL      | A5 (or D22 on ESP32) |

> ⚠️ Make sure your display is using I2C. SPI displays are not supported in this sketch.

## 🚀 Upload and Run

1. Open the Arduino IDE.
2. Load the `bongo_cat.ino` file (from this repo).
3. Connect your board via USB.
4. Select the correct board and COM port from **Tools > Board** and **Port**.
5. Click the **Upload** button.

You should now see the Bongo Cat animation on your OLED screen!

## 🖼️ Customize Frames

To create your own animations:
- Convert your bitmap images (monochrome, 128x64px) to byte arrays using tools like:
  - [Image2CPP](https://javl.github.io/image2cpp/)
- Replace or add new frames in the sketch using `PROGMEM`.

## 🧠 Credits

- Bongo Cat character inspired by the internet meme & animations.
- Libraries by [Adafruit](https://adafruit.com).

## 📝 License

Feel free to use and modify for personal or educational use.

---

Happy bongo-ing! 🐱🥁
