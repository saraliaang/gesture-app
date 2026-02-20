# 🖐️ Gesture Lab

<div align="center">
  <img src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E" alt="JavaScript" />
  <img src="https://img.shields.io/badge/MediaPipe-00B4EB?style=for-the-badge&logo=mediapipe&logoColor=white" alt="MediaPipe" />
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
</div>

<br/>

> **The Thesis:** Touchscreens restrict how we interact with digital interfaces, limiting input to taps and swipes even as devices grow more capable. Users crave more natural, expressive interactions beyond glass and buttons.

**Gesture Lab** is an experimental frontend prototype exploring hands-as-input interactions. It serves as the foundational gesture-recognition engine that ultimately powers my immersive, gesture-controlled portfolio experience. 

---

## 📸 Video Demo
https://github.com/user-attachments/assets/5a31c939-1863-4731-8cc7-9622f05f2086
---

## 🧠 Design Intent & Problem Space

This lab was created to establish a reliable interaction language that can scale into real-world, camera-driven experiences. Through iterative testing, the gesture set was intentionally refined to prioritize:
1. **Learnability:** Gestures that feel intuitive and mimic natural human movements.
2. **Noise Resilience:** Ensuring the camera does not misinterpret casual hand movements.
3. **Accessibility:** Providing a seamless mouse fallback for hybrid interaction.

## 🔣 The Core Gesture Vocabulary

Real-time camera input and hand tracking were utilized to map specific hand states to UI actions:

* 🟢 **Wake:** Activates the tracking camera and initiates the on-screen cursor.
* ↕️ **Scroll:** Hand tracking mapped to carousel or panel navigation.
* ✋ **Summon:** A closing palm moving away from camerag(like grabbing) - pull up menus or hidden UI elements.
* 💨 **Dismiss:** A palm opening and moving closer to the camera(like throwing) - sweeping motion to exit or cancel overlays.

## 🛠 Technical Execution

* **AI Vision Integration:** Integrated Google's **MediaPipe** to handle real-time hand-landmark detection via webcam.
* **Custom Cursor Mapping:** Engineered JavaScript logic to translate 3D spatial coordinates from the camera into a smooth, 2D visual cursor on the DOM.
* **State Management:** Built a robust event-listening system to track continuous gesture states (e.g., holding a pinch) versus discrete triggers (e.g., a single swipe).
* **On-Screen Guidance:** Developed a cinematic "Gesture Guide" overlay with clear iconography to support user onboarding.

## 🚀 Setup & Installation

To run this experimental lab locally:

1. Clone the repository and navigate to the project directory
-  apps/gesture-lab
2. Install dependencies:
```bash
   npm install
   ```
3. Start the dev server:

```bash
   npm run dev
   ```

