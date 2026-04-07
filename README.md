# Pomodoro Timer Chrome Extension

A simple and effective Pomodoro timer Chrome extension to help you focus and get things done!

## Features

- **Customizable Timer Duration**: Set your preferred Pomodoro session length (1-60 minutes)
- **Visual Timer Display**: Clean, large countdown display showing remaining time
- **Start/Pause/Reset Controls**: Full control over your timer sessions
- **Task Management**: Add, edit, and delete tasks to keep track of your work
- **Desktop Notifications**: Get notified when your Pomodoro session is complete
- **Persistent Storage**: Your tasks and timer settings are saved automatically
- **Beautiful UI**: Modern, clean interface with an intuitive red and white color scheme

## Installation

### From Source

1. Clone this repository:
   ```bash
   git clone https://github.com/vasylpryimakdev/pomodoro-timer.git
   cd pomodoro-timer
   ```

2. Open Chrome and navigate to `chrome://extensions/`

3. Enable "Developer mode" in the top right corner

4. Click "Load unpacked" and select the `start` directory

5. The Pomodoro Timer extension should now appear in your extensions list and toolbar

## Usage

### Basic Timer Operation

1. **Start Timer**: Click the extension icon in your Chrome toolbar, then click "Start Timer"
2. **Pause Timer**: Click "Pause Timer" to temporarily stop the countdown
3. **Reset Timer**: Click "Reset Timer" to return to the full session duration
4. **Notification**: When your session ends, you'll receive a desktop notification

### Customizing Timer Duration

1. Right-click the extension icon and select "Options"
2. Enter your preferred session length (1-60 minutes)
3. Click "Save Options"
4. The timer will use your new duration for future sessions

### Managing Tasks

1. **Add Task**: Click "Add Task" to create a new task input field
2. **Edit Task**: Type directly in any task field to edit it
3. **Delete Task**: Click the "X" button next to any task to remove it

## Technical Details

### Permissions

The extension requires the following permissions:

- **storage**: To save timer state, tasks, and user preferences
- **alarms**: To run the timer in the background
- **notifications**: To alert you when timer sessions complete

### File Structure

```
pomodoro-timer/
|
| manifest.json          # Extension manifest
| background.js          # Service worker for timer logic
| icon.png              # Extension icon
|
| popup/                # Timer popup interface
|   popup.html
|   popup.css
|   popup.js
|
| options/              # Settings page
|   options.html
|   options.css
|   options.js
```

### Key Components

- **Background Service Worker**: Handles timer countdown and notifications
- **Popup Interface**: Main timer display and controls
- **Options Page**: User settings and preferences
- **Storage System**: Persistent data for tasks and settings

## Development

### Local Development

1. Make changes to the source files
2. Go to `chrome://extensions/`
3. Click the refresh icon on your extension
4. Test your changes

### Code Style

The extension follows standard JavaScript conventions with:
- Consistent indentation
- Clear function naming
- Modular structure
- Modern ES6+ features

## About

This Pomodoro Timer extension was created to help improve productivity and focus using the Pomodoro Technique. The Pomodoro Technique is a time management method that uses a timer to break work into intervals, traditionally 25 minutes in length, separated by short breaks.

---

**Made with focus and productivity in mind!**
