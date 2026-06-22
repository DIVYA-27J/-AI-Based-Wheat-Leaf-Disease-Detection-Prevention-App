# AgriVision | Wheat Disease AI

AgriVision is an AI-based progressive web application (PWA) designed to detect diseases in wheat leaves using machine learning directly in the browser. 

## Features
- **In-Browser Inference:** Uses TensorFlow.js to run the disease detection model locally on your device, ensuring privacy and speed.
- **Multilingual Support:** Available in English, Tamil (தமிழ்), and Hindi (हिन्दी) for wider accessibility.
- **Progressive Web App (PWA):** Can be installed on mobile and desktop devices and works seamlessly offline.
- **Camera & Gallery Support:** Capture a live photo using your device's camera or upload an existing image from your gallery.
- **Read Aloud:** Accessibility feature to read out the diagnosis and treatment advice.

## Getting Started

Since this is a static web application, it needs to be served via a local web server to function properly (especially for the service worker and camera permissions to work securely).

### Prerequisites
- Node.js (which includes `npx`)

### How to Run Locally

1. Open your terminal and navigate to this folder.
2. Run the following command to start a local server:
   ```bash
   npx http-server .
   ```
3. Open your web browser and go to `http://127.0.0.1:8080`.

## Architecture
- **HTML/CSS:** Structure and styling (Outfit font, Material Icons).
- **JavaScript (`app.js`):** Core logic for camera access, language translation, image processing, and TensorFlow.js model integration.
- **Service Worker (`sw.js` & `manifest.json`):** Enables offline functionality and PWA installation.
