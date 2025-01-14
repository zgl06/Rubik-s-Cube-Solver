# Rubik's Cube Solving Robot

A LEGO EV3-based robotic system that can automatically solve a Rubik's cube. The robot combines mechanical manipulation with computer vision to scan, process, and physically solve a Rubik's cube.

## Components

- **Hardware**: LEGO EV3 brick, 3 motors for cube manipulation, color sensors for face detection, and ultrasonic sensor for cube presence detection
- **Software**: C programs for robot control and Python script for solution generation

## Files

- `runRobot.c`: Main control program for the EV3 robot, handles mechanical movements and user interface
- `main.py`: Web scraping solution finder using Selenium
- `readandwritefile.c`: Manages file I/O operations and cube state data
- `PC_FileIO.c` & `EV3_FileIO.c`: Utility files for PC-EV3 file compatibility
- Data files: `scramble.txt` (scramble sequence), `output.txt` (solution sequence)

## Setup

1. Install required Python package:
```bash
pip install selenium
```

2. Load programs onto EV3 brick

## Usage

1. Power on EV3 brick
2. Place cube in robot holder
3. Use EV3 buttons:
   - Left/Right: Scramble cube
   - Enter: Scan and solve cube
   - Down: Exit program

## Move Notation

- Basic moves: U (Up), D (Down), F (Front), B (Back), L (Left), R (Right)
- Direction: 0 = clockwise, 1 = counter-clockwise

## Features

- Autonomous cube solving
- Random scramble generation
- Real-time color sensing
- Solution time tracking
- Safety features (ultrasonic detection, error handling)
