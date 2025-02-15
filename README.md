# Motion-Controlled Sound

## Overview

The **Motion-Controlled Sound** app is a web-based application that utilizes motion sensors from mobile devices to dynamically control sound properties. By tilting the device, users can modify the pitch and volume of an oscillator in real-time.

## Features

- **Motion-Sensor Integration**: Uses device motion (tilt) to adjust sound properties.
- **Dynamic Sound Control**: Modifies pitch and volume based on device orientation.
- **User Permissions Handling**: Requests permission to access motion sensors on iOS.
- **Simple UI**: Buttons to enable motion sensors and toggle sound.
- **Real-Time Feedback**: Displays pitch and volume values on-screen.

## Technologies Used

- **HTML**: Structure and UI components.
- **CSS**: Styling and layout.
- **JavaScript**: Handles motion tracking, audio processing, and user interactions.
- **Web Audio API**: Generates and modifies sound in real-time.

## Installation & Usage

1. **Download or Clone the Repository**
   ```sh
   git clone https://github.com/your-repo/motion-sound-audio.git
   cd motion-sound-app
   ```

2. **Open the `index.html` File in a Browser**
   - The app works best on **mobile devices** with motion sensors.
   - For iOS devices, ensure that **motion permissions** are enabled in settings.

3. **Usage Instructions**
   - Click **"Enable Motion Sensors"** to grant access.
   - Click **"Start Sound"** to begin sound playback.
   - Tilt your device **forward/backward** to adjust pitch.
   - Tilt your device **sideways** to modify volume.

## File Structure

```
motion-sound-app/
│── index.html   # Main HTML file
│── style.css    # Stylesheet for UI
└── script.js    # JavaScript logic for sound and motion tracking
```

## How It Works

- **Motion Permission Request**: On iOS, the app requests user permission to access motion sensors.
- **Audio Initialization**: When the user clicks "Start Sound," an oscillator is created.
- **Motion-Based Sound Control**:
  - **Pitch** (Hz) is adjusted based on **front/back tilt** (`event.beta`).
  - **Volume** is modified based on **side tilt** (`event.gamma`).

## Known Issues & Limitations

- **Browser Support**: Works best in **mobile browsers** like Chrome or Safari.
- **Desktop Compatibility**: Limited functionality on non-mobile devices (no motion sensors).
- **iOS Restrictions**: Requires user interaction to enable sound (Web Audio API limitations).

## License

This project is open-source and free to use under the MIT License.

---

🎵 **Enjoy experimenting with motion-controlled sound!**
