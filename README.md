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

A singleton-based bridge that exposes MediaPipe hand landmark data to other scripts.

```csharp
// Get joint position
HandDataProvider.Instance.TryGetJointPosition(0, 8, out Vector3 position);

// Get distance between two joints
HandDataProvider.Instance.TryGetJointDistance(0, 8, 1, 4, out float distance);

// Get midpoint between two joints
HandDataProvider.Instance.TryGetJointMidpoint(0, 8, 1, 4, out Vector3 center);
