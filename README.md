# Device Shake Counter

This is a React application that counts sharp device shakes using data from the device's accelerometer or gyroscope. Each detected shake increments a counter displayed on the screen, and an animation provides visual feedback for each shake event.

## Features

- **Shake Counter**: Counts each sharp shake based on device motion data.
- **Shake Animation**: Provides a visual cue (e.g., color flash or shake) for each detected shake.
- **Error Handling**: Displays an error message if the device does not support motion sensors or if sensor access is denied.

## Technologies Used

- **React**: Frontend library for building user interfaces.
- **TailwindCSS**: Utility-first CSS framework for styling.
- **Sensors API**: For accessing device motion data.

## Getting Started

### Prerequisites

- **Node.js** (v12 or higher recommended)
- **npm** (Node Package Manager)

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/device-shake-counter.git
   cd device-shake-counter
2. Install the dependencies:
   ```bash
   npm install
3. Start the development server:
   ```bash
   npm start

The app will be running at http://localhost:3000.

### Shake Detection Logic
This app uses the DeviceMotionEvent API to track changes in acceleration along the X, Y, or Z axes. A "shake" is defined as a rapid change of more than 15 m/s² on any of these axes, indicating a strong shake movement. Each time a shake is detected, the counter increments by 1, and the animation responds to give visual feedback.

### Usage
Shake your device: The shake counter will increment with each detected shake, and an animation will respond to the shake event.
Reset Counter: Press the "Reset Counter" button to reset the shake count to zero.
Error Handling: If motion sensors are not supported or access is denied, an error message will appear.

### Troubleshooting
Permissions: On iOS devices, make sure to enable "Motion & Orientation Access" under Settings > Safari.
Testing on iOS: Note that Chrome on iOS also follows Safari’s motion permission settings due to iOS’s WebKit restrictions.

### Link to the Deployed App
https://device-shake-counter.vercel.app/