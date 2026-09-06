# Pull

A real-time computer-vision piece where hand gestures control a generative particle field — pinch to gather and compress particles into clusters, release to let them scatter. Built with React and MediaPipe Hands, running entirely in-browser.

*Status: Towards the end of development. Architecture and interaction design below reflect the current plan; see Build Progress and Mockup.*

<img width="986" height="754" alt="image" src="https://github.com/user-attachments/assets/c20f2f99-133f-4317-8221-3662f8930a88" />


## Tech Stack
React · MediaPipe Hands · JavaScript · Canvas · Vercel · React Testing Library

## Concept
A user's bare hand becomes the only control surface for a field of generative, data-driven forms, pinch to gather them into controlled clusters, release to let them scatter into ungoverned motion. The goal is to make an abstract idea (the tension between control and entropy) something felt physically with your hands, not just read about or watched.

## What This Demonstrates
- Real-time computer vision integration, consuming MediaPipe's hand-landmark output live in-browser
- React state management (hooks) synchronizing camera input, gesture data, and canvas rendering
- Custom gesture math: Euclidean distance between hand landmarks, coordinate-space conversion, frame-to-frame smoothing
- Performance-conscious rendering, running ML inference and animation concurrently
- Component testing (React Testing Library) for gesture-to-state logic

## Build Progress
- [ ] Hand-tracking hook + pinch-distance calculation
- [ ] Single-shape gesture mapping (proof of concept)
- [ ] Full particle system + cluster/scatter behavior
- [ ] Performance tuning
- [ ] Visual design pass + cross-device testing
- [ ] Deploy + demo video

## A Note on Status
This is my most technically ambitious project to date and would love any tips on media pipe.
