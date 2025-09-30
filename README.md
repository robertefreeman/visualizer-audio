# visualizer-audio

A web-based 3D audio visualizer that uses Babylon.js to create stunning real-time visualizations of sound captured from your microphone.

## Features

- 🎵 Real-time audio visualization using microphone input
- 🎨 3D graphics powered by Babylon.js
- 🌈 Colorful frequency bars arranged in a circular pattern
- ⚡ Smooth animations and responsive design
- 🎮 Interactive camera controls (zoom, rotate, pan)
- 🔊 Web Audio API integration for audio analysis

## How to Use

1. Open `index.html` in a modern web browser (Chrome, Firefox, Edge, or Safari)
2. Click the "Start Visualizer" button
3. Allow microphone access when prompted by your browser
4. Make some noise! Speak, play music, or create sounds to see the visualization respond

## Technical Details

- **Babylon.js**: Used for 3D rendering and scene management
- **Web Audio API**: Captures and analyzes audio from the user's microphone
- **FFT Analysis**: Converts audio signals into frequency data for visualization
- **64 Frequency Bars**: Each bar represents a different frequency range
- **Central Sphere**: Responds to overall audio volume

## Browser Compatibility

This application requires:
- A modern web browser with WebGL support
- Microphone access permissions
- JavaScript enabled

Tested on:
- Chrome 90+
- Firefox 88+
- Edge 90+
- Safari 14+

## Privacy

This application:
- Only accesses your microphone when you click "Start Visualizer"
- Does NOT record or store any audio data
- Does NOT transmit audio data over the network
- All processing happens locally in your browser

## Development

This is a standalone HTML application with no build process required. 

### Running Locally

**Option 1: Direct file access (simplest)**
Simply open `index.html` directly in your web browser. Note: Some browsers may restrict microphone access for file:// URLs.

**Option 2: Local web server (recommended)**
```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (http-server package)
npx http-server -p 8000
```

Then navigate to `http://localhost:8000` in your browser.

### Dependencies

The application loads Babylon.js from a CDN. If you need to run this offline or in an environment without internet access:

1. Download Babylon.js: https://cdn.babylonjs.com/babylon.js
2. Save it in the same directory as index.html
3. Update the script tag in index.html to: `<script src="babylon.js"></script>`

## License

MIT License - See LICENSE file for details