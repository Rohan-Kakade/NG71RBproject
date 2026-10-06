# NG71RBproject

Sample Mbed CE project for the STM32 NUCLEO-G071RB development board using PlatformIO and Visual Studio Code.

This repository provides a starter project for students and developers wishing to use Mbed CE with PlatformIO in VS Code.

## Requirements

Before using this project, install:

- Visual Studio Code
- PlatformIO IDE extension
- Git

## Hardware

- STM32 NUCLEO-G071RB development board
- USB cable

## Getting Started

### Clone the Repository

Open a terminal and run:

```bash
git clone https://github.com/Rohan-Kakade/NG71RBproject.git
```

Navigate to the project folder:

```bash
cd NG71RBproject
```

Open the project in VS Code:

```bash
code .
```

Alternatively:

1. Open VS Code.
2. Press `Ctrl + Shift + P`.
3. Select **Git: Clone**.
4. Enter:

   ```text
   https://github.com/Rohan-Kakade/NG71RBproject.git
   ```

5. Choose a destination folder.
6. Open the cloned repository when prompted.

## Project Structure

```text
NG71RBproject/
│
├── include/
├── lib/
├── src/
│   └── main.cpp
├── test/
├── platformio.ini
└── README.md
```

### Folder Description

| Folder | Purpose |
|----------|----------|
| src | Application source code |
| include | Header files |
| lib | Custom libraries |
| test | Unit tests |
| platformio.ini | PlatformIO project configuration |

## Building the Project

Click the **Build** button (✓) in the PlatformIO toolbar.

Alternatively, use:

```bash
pio run
```

## Uploading to the Board

1. Connect the NUCLEO-G071RB via USB.
2. Press the **Upload** button (→) in the PlatformIO toolbar.

Or use:

```bash
pio run --target upload
```

## Serial Monitor

Open the PlatformIO Serial Monitor using:

```bash
pio device monitor
```

If your project uses a different baud rate, update the `platformio.ini` file accordingly:

```ini
monitor_speed = 9600
```

## PlatformIO Configuration

This project uses:

```ini
board = nucleo_g071rb
framework = mbed-ce
upload_protocol = mbed
```

## Creating Your Own Project

To use this repository as a starting template:

1. Clone the repository.
2. Rename the project folder if required.
3. Modify the source code in `src/main.cpp`.
4. Commit and push changes to your own GitHub repository.

## Useful Commands

Build:

```bash
pio run
```

Upload:

```bash
pio run --target upload
```

Clean:

```bash
pio run --target clean
```

Monitor Serial Output:

```bash
pio device monitor
```

## License

This project is provided for educational purposes.
