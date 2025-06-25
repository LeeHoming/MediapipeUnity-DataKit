# MediapipeUnity-DataKit


**MediapipeUnity-DataKit** is a lightweight Unity toolkit for structured access to hand, face, and body tracking data based on [MediaPipeUnityPlugin](https://github.com/homuler/MediaPipeUnityPlugin).

This package simplifies the use of MediaPipe tracking results by exposing a clean C# API for retrieving joint positions, computing distances and midpoints, and triggering interaction events.

---

## Features

- Strict, modular data access for hand landmarks
- Public API for joint positions, distances, and midpoints
- Component for triggering events when joints cross distance thresholds
- Optional debug visualization using `RawImage` overlay
- Designed for future support of face and body tracking

---

## Dependencies

- [homuler/MediaPipeUnityPlugin](https://github.com/homuler/MediaPipeUnityPlugin)
- Tested on version **v0.16.1**

---

## Components

### `HandDataProvider.cs`

