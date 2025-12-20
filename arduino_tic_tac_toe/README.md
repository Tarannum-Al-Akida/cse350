## Arduino Tic-Tac-Toe (Uno + 20x4 I2C LCD + 4x4 Keypad)

This matches the setup described in your PDF: a 2-player Tic-Tac-Toe game where players press keypad keys **1–9** to place **X/O**, and the 20×4 LCD shows the grid + status.

### Wiring (from your PDF)

#### 4x4 Keypad → Arduino Uno

Connect keypad **pins 1–8** to **D2–D9**:
- Keypad pin 1 → D2
- Keypad pin 2 → D3
- Keypad pin 3 → D4
- Keypad pin 4 → D5
- Keypad pin 5 → D6
- Keypad pin 6 → D7
- Keypad pin 7 → D8
- Keypad pin 8 → D9

> Assumption used in the sketch (typical): keypad pin order is **R1 R2 R3 R4 C1 C2 C3 C4**.

#### I2C LCD (with I2C backpack) → Arduino Uno
- **SDA** → **A4**
- **SCL** → **A5**
- **VCC** → **5V**
- **GND** → **GND**

### Controls
- **1–9**: place mark in that cell
- **#**: reset (also auto-resets 5s after win/tie)

### Arduino Libraries
Install from **Tools → Manage Libraries…**
- **Keypad** (Mark Stanley, Alexander Brevig)
- **LiquidCrystal I2C** (common versions work; the sketch includes `LiquidCrystal_I2C.h`)

### Notes / Troubleshooting
- If the LCD backlight turns on but text doesn’t show, your I2C address may be `0x3F` instead of `0x27`.
  - Change `LCD_ADDR` in `arduino_tic_tac_toe.ino`.

