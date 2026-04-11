# Spatial Interaction Workspace

An advanced, gesture-controlled 3D web workspace built with **Three.js** and **MediaPipe**. This application allows users to spawn, select, transform, and combine 3D objects in real-time using hand gestures from an ordinary webcam.

## Features

- **Gesture Control**: Leverages `MediaPipe Hands` to identify pinch and point gestures, transforming your index finger and thumb into a spatial cursor.
- **Holographic 3D Environment**: Implements `Three.js` Post-Processing techniques (like UnrealBloom) over a transparent grid and custom shading, creating a cinematic, tech-noir aesthetic.
- **Dynamic Transforms**:
  - `Move`: Grab an object by pinching and move it seamlessly across a dynamic 3D depth plane.
  - `Rotate`: Twist and turn objects based on relative hand translations.
  - `Scale`: Intuitively shrink and grow objects via vertical hand shifts.
- **Shape Builder**: Point your index finger upward to instantly summon primitives (Cubes, Spheres, Cones, Cylinders, Tori).
- **Combine/Merge System**: Pinch an object and physically drag it into another to hierarchically link them together. The resulting composition can be manipulated as a single structural unit. 
- **Scene Memory**: Save and dynamically reconstruct highly customized spatial scenes inside the browser's persistent `localStorage`, fully retaining scale, rotation, and complex grouped arrays.

## Tech Stack

- **Vanilla HTML/CSS/JS**
- [**Three.js**](https://threejs.org/) (Core WebGL rendering, Post-Processing)
- [**MediaPipe**](https://developers.google.com/mediapipe) (Machine Learning Hand Tracking)
- [**Tailwind CSS**](https://tailwindcss.com/) (Rapid responsive UI)

## Getting Started

Because MediaPipe requires secure contexts to access the device camera, the simplest way to run this locally is to use a basic web server.

1. Clone the repository:
   ```bash
   git clone https://github.com/shanmugamani45/spatial-interaction-workspace.git
   cd spatial-interaction-workspace
   ```
2. Serve the directory:
   You can use Node.js (`npx serve`), Python (`python -m http.server`), or VSCode's Live Server extension.
   - Using Python: `python -m http.server 8000`
   - Using Node: `npx serve .`
3. Navigate to `http://localhost:8000` (or your specific server port) in your web browser.
4. Allow camera permissions when prompted.
5. Raise your hand in view of the webcam and begin!

## Gestures Reference

- **Create**: Curl all fingers except your Index finger straight up. Hold for 0.3s.
- **Grab / Interact**: Bring your Thumb and Index finger together to pinch an object on the spatial cursor.

## Live Demo 
https://spatial-interaction-workspace.vercel.app/

## ScreenShots
<img width="1903" height="937" alt="image" src="https://github.com/user-attachments/assets/e9344f6f-bf3e-425b-b0d6-adcef1a59f94" />

<img width="1919" height="969" alt="image" src="https://github.com/user-attachments/assets/4c72e08d-4967-4fd3-bcaa-ae217cb9412c" />

## License

This project is open-source and free to modify.
