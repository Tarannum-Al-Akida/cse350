🎮 Arduino Tic-Tac-Toe Game using OLED Display and Keypad
📌 Project Overview
This project implements a Tic-Tac-Toe game on an Arduino Uno using a 4x4 keypad for input and a 128x64 OLED display for visual output. Two players can play the classic Tic-Tac-Toe game by pressing keys 1–9 on the keypad to place their marks (X or O) on the board.
The system displays the game board, player turns, and the winner directly on the OLED screen.
This project was developed for the CSE350 course to demonstrate the integration of embedded systems, hardware interfaces, and game logic using Arduino.
⚙️ Hardware Components
Component	Description
Arduino Uno	Main microcontroller
128x64 OLED Display (SSD1306)	Displays the game board
4x4 Keypad	Player input
Jumper Wires	Connections between components
Breadboard	Circuit setup
📚 Libraries Used
Make sure the following Arduino libraries are installed:
SPI.h
Wire.h
Adafruit_GFX.h
Adafruit_SSD1306.h
Keypad.h
You can install them from the Arduino Library Manager.
