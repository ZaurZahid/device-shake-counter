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
   git clone https://github.com/YOUR_USERNAME/device-shake-counter.git
   cd device-shake-counter
2. Install the dependencies:
   npm install
3. Start the development server:
   npm start

The app will be running at http://localhost:3000.