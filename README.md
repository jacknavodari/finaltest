# FinalTestApp - AI-Powered Windows App Builder

FinalTestApp is an Electron application designed to help developers create new Windows applications enhanced with AI capabilities. This tool provides an interface to integrate AI models like Gemini, Claude, and Qwen into Windows applications.

## Features

- Create Windows applications with integrated AI capabilities
- Interface with popular AI models (Gemini, Claude, Qwen)
- Cross-platform development framework
- Dark mode support for comfortable development
- Modern UI with customizable interface
- Local storage for saving project configurations

## How It Works

FinalTestApp serves as a development environment where users can:
- Design application interfaces
- Integrate AI model APIs
- Build and package Windows applications
- Test AI features before deployment

## Prerequisites

Before you begin, make sure you have Node.js installed on your system.
- Node.js (version 14 or higher)
- npm (usually comes with Node.js)

## Installation

1. Make sure you have Node.js installed on your system. You can download it from [nodejs.org](https://nodejs.org/)

2. Clone or download this repository to your local machine

3. Navigate to the project directory:
   ```bash
   cd FinalTestApp
   ```

4. Install the required dependencies:
   ```bash
   npm install
   ```

## Running the Application

To run the application in development mode:
```bash
npm start
```

This will launch the Electron application with your schedule.

## Building the Application

### Method 1: Using NPM Scripts
To create a distributable version of the application:
```bash
npm run build
```

### Method 2: Using Build Scripts
Windows users can use the provided batch files:
- Double-click `build_installer.bat` to install dependencies and build the application
- Alternatively, double-click `install_and_build.ps1` (PowerShell script) to build with more detailed output

The built application will be available in the `release` directory as an installer for your platform.

### Available Build Scripts
- `npm run build` - Creates a distributable installer for your platform
- `npm run pack` - Creates a packaged app without installer (for testing)
- `npm run dist` - Same as build command

### Supported Platforms
- Windows: NSIS installer (.exe)
- macOS: DMG image (.dmg)
- Linux: AppImage (.AppImage)

## Usage

- Click on the day tabs at the top to view the schedule for that day
- The "Orar" button toggles between schedule views
- Use the pencil icon to edit the student name
- The moon/sun icon toggles dark mode
- Click "Adaugă Eveniment" to add custom events to a specific day
- Events are saved in your browser's local storage
- The status bar at the top shows the current active class or upcoming classes

## Customization

The schedule can be customized by modifying the `schedule` array in the index.html file. The teachers list can be updated in the same manner in the `teachers` array.

## Troubleshooting

If the application fails to start, make sure:
- Node.js and npm are correctly installed
- All dependencies are installed using `npm install`
- Your system meets the minimum requirements for Electron
- Run `npm install` again if you encounter issues

If building fails:
- Make sure you have enough disk space in the temp directory
- Try running the build command as administrator (Windows)
- Check that your antivirus isn't blocking the build process

## License

MIT
