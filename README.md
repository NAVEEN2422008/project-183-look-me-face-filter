# C183 - "Look Me" Face Filter App

A React Native (Expo) augmented-reality face-filter camera app that overlays animated accessory filters (crowns, flowers, hair, hats, and more) on detected faces in real time.

## Features

- Real-time **face detection** using `expo-camera` + `expo-face-detector`
- **AR filters** anchored to eye and nose landmarks via the `Filter` component
- Filter categories: Crown, Flowers, Hairs, Hats, Others (11+ filter variations)
- Horizontal category and filter pickers with per-filter positioning configs
- Front camera with fast face-detection settings and landmark classification

## Tech Stack

- **React Native** 16.13.1 / **Expo** SDK 41
- **expo-camera**, **expo-face-detector**, **expo-status-bar**
- **react-native-responsive-fontsize** for responsive sizing

## Project Structure

```
├── App.js                 # Root component (renders Main)
├── screens/Main.js        # Camera screen, face detection, filter pickers
├── components/Filter.js   # Overlays a filter image aligned to detected face
├── app.json               # Expo app configuration
└── assets/                # Filter images (crowns, flowers, hats, etc.)
```

## Installation

1. Clone the repository.
2. Install dependencies:

```bash
cd c184
yarn install
```

## Usage

Start the Expo dev server:

```bash
yarn start        # or: npx expo start
yarn android      # run on Android
yarn ios          # run on iOS
```

1. Grant camera permission when prompted.
2. Point the front camera at a face to see filters snap onto it.
3. Tap a category, then a filter thumbnail to switch the applied overlay.
