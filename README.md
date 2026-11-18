# Vision Enhancement for an XR Headset

**2024 XR Device Content Makerthon & Ideathon (Pangyo, Nov 2024) — team 3DOS; I owned all development and the on-stage demo. The code was lost; this repository holds a summary, headset captures and the slide pages with my own work.**

Two published imaging methods from Prof. Myungjin Cho's research, Fourier peplography for fog and photon counting for low light, ported to C++/OpenCV as an Android native plugin for a Unity app and run live on the Metalens 2 headset's own camera.

**Write-up:** listed under other work on the site ([English](https://zoocasso.github.io/en/work/) · [한국어](https://zoocasso.github.io/work/))

<img src="docs/headset-demo.webp" alt="Screen recording from inside the headset, left eye: a hand presses the app's buttons; a dark room turns into a noisy but visible image with photon counting, and a fogged water tank becomes clearer with Fourier peplography" width="720">

<sub>Recorded inside the headset (left eye) while the app ran: pressing its buttons by hand switches on photon counting in a dark room, then Fourier peplography on a fogged water tank. The stretches before each button press play at 2× speed; the frames are not edited. The frame rate was not measured.</sub>

- **The methods are not mine.** Both are published work from Prof. Myungjin Cho's research.
- **My part was the port.** I wrote both in C++/OpenCV, built them as an Android native plugin and wired it into a Unity app, so that they ran live on the headset. It was my first real-time implementation of them on a device.
- **The image quality is limited by the headset.** Its camera gives a low-resolution image, so the results are rough: they show the methods running live on the device, not their best quality.

<img src="docs/diagram.png" alt="Headset camera frames go through the native C++/OpenCV plugin inside the Unity app to the headset display" width="780">

<sub>Solid blue: my work · grey dashed: others' work (published methods) · white: device.</sub>

| At&nbsp;a&nbsp;glance | |
| :--- | :--- |
| **What** | Fog and smoke removal (Fourier peplography) and low-light recovery (photon counting), run live on the headset's own camera feed |
| **My part** | The port and all of the development: the C++/OpenCV implementation, the Android native build and the Unity integration. Also the presentation and the on-stage demo |
| **Others** | The two methods are published work from Prof. Myungjin Cho's research. Team 3DOS: five members of my undergraduate lab were registered |
| **Numbers** | None: the frame rate was not measured, and the code was lost |
| **Stack** | C++, OpenCV 3.4.16, Android native plugin (arm64-v8a), Unity 2021.3 (IL2CPP), Metalens 2 |
| **Run · tests** | Not runnable: the source code was lost. The slide pages with my own work are in [`slides-excerpt.pdf`](slides-excerpt.pdf) |

## What I built

- **Both methods, written from scratch in C++/OpenCV** from the published work.
- **An Android native plugin inside a Unity app.** The code was built as a `.so` for arm64-v8a and loaded by a Unity (IL2CPP) app that reads the headset camera and shows the result on the headset display.
- **Only the headset's own camera.** No extra sensors or light sources: each frame of the camera feed is processed on the device.

How the two methods work:

- **Fog and smoke (Fourier peplography):** the frame is Fourier-transformed, a filter attenuates the low-frequency part that the scattering medium adds, and the inverse transform gives the clearer image.
- **Low light (photon counting):** the scene is recovered from the very few photons a dark frame contains, by statistical estimation (maximum likelihood).

Uses proposed in the presentation: fire scenes, foggy roads, dark outdoor work sites, wildlife filming, night-time surveillance and night driving.

## Captures from the headset

Still frames taken through the device SDK (left eye only).

<img src="docs/headset-before-after.webp" alt="Headset captures with a moving divider: the camera feed on its left, the processed frame on its right. Light fog and Fourier peplography, then lights off and photon counting" width="820">

<sub>Left of the divider is the camera feed, right of it the processed frame; the captures themselves are not edited. With the lights off the camera feed is almost black.</sub>

<img src="docs/headset-results.jpg" alt="Headset captures: a scene without fog, with light fog, and with light fog after Fourier peplography; a room with lights on, lights off, and lights off after photon counting" width="820">

<sub>Each row is one scene, with the unprocessed reference on the left (no fog; lights on).</sub>

## The event

- **Event:** 2024 XR Device Content Makerthon & Ideathon, Makerthon track, finals at the Pangyo Metaverse Hub, November 2024. Teams built content for the Metalens 2 headset.
- **Team:** 3DOS. Five members of my undergraduate lab (3D Image Processing Systems Lab, Hankyong National University) were registered as the team; I did all of the development and gave the presentation and the on-stage demo.
- **This repository:** this summary and the slide pages with my own work. The source code was lost, so it is not included.

<details>
<summary><b>About the slides</b></summary>

[`slides-excerpt.pdf`](slides-excerpt.pdf) holds the 12 of the 24 presented slides that contain only my own material: the title, how the idea differs from existing systems, the build diagram, and the captures from the headset taken through the device SDK (fog: none, light, light + Fourier peplography, thick, thick + Fourier peplography; low light: lit, dark, dark + photon counting).

</details>

## On stage

<img src="docs/on-stage.jpg" alt="Presenting the title slide, Real-time Vision Enhancement Device by 3DOS, at the lectern of the finals stage" width="600">

<sub>The presentation at the finals, November 2024.</sub>
