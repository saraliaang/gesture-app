# Gesture App

A standalone gesture-driven interface prototype extracted from sara-porfolio-hub-.

## Product Requirements

### Goal
Build a self-contained gesture interaction demo that can be tested and tuned independently, then integrated into other experiences (e.g., Sara-s-hub-).

### Core Features
- Camera hand-tracking input with on-screen preview.
- Gesture recognition for wake, confirm, scroll, summon, dismiss.
- Visual cursor mapped to hand position with configurable sensitivity and smoothing.
- Gesture guild overlay (help UI) with clear iconography and descriptions.
- Mouse fallback for interaction and toggles.

### User Flow
1. User enables gesture mode.
2. Camera preview shows hand tracking and current gesture state.
3. User performs gestures to move the cursor and trigger actions.
4. User can open the gesture guild to learn commands.

### Interaction Rules
- Summon/confirm gestures trigger primary actions.
- Dismiss gesture exits or cancels overlays.
- Scroll gestures allow carousel/panel navigation.
- Mouse remains a fallback when gestures are off.

### Visual Requirements
- On-brand, high-contrast UI with cinematic overlays.
- Always-visible system status and gesture feedback.
- Subtle motion that explains gestures without overwhelming the scene.

### Non-Goals
- No backend services.
- No long-term storage or auth.

## Setup

1. Install dependencies:
   ```bash
   npm install
   ```
2. Start the dev server:
   ```bash
   npm run dev
   ```

## Notes

- The repo mirrors `sara-porfolio-hub-` as a standalone project.
- Tune gesture sensitivity in the gesture controller logic as needed.
