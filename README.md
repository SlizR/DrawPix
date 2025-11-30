# DrawPix: A Digital Canvas by Sliz®

<p align="center">
  <img src="https://img.shields.io/badge/Wayback Machine-Live-brightgreen" alt="Project Status: Live">
  <img src="https://img.shields.io/badge/Canvas%20Size-800x800-blueviolet" alt="Canvas Size">
  <img src="https://img.shields.io/badge/Pixels-25600-red" alt="Total Pixels">
  <img src="https://img.shields.io/badge/Website-drawpix.space-blue" alt="Total Pixels">
</p>

---

## 💡 About DrawPix

**DrawPix** is a collaborative digital art platform designed as an engaging, large-scale pixel canvas. It provides users with a unique opportunity to contribute a single, permanent pixel to a massive **800x800 grid**, resulting in a final image of **25,600 individual pixels**.

The purpose of DrawPix is simple: **create a lasting digital story**. Every pixel placed is a permanent mark, building a shared, evolving masterpiece over time. The project is designed to be interactive, visually rewarding, and accessible to users on both desktop and mobile devices.

Official website of pixels: [DrawPix](https://drawpix.space)

### Key Features:

* **Massive Canvas:** A total of 25,600 available pixels to color.
* **Persistent Data:** Pixels are permanently saved via a backend worker.
* **Ad-Supported Interaction:** Placing a pixel requires a quick ad view to support server resources and ensure fair use.
* **Intuitive Controls:** Optimized for seamless panning, zooming, and drawing on any device.

---

## 🚀 User Guide: How to Place Your Pixel

DrawPix is built for simplicity. Follow these steps to select your spot, choose a color, and place your permanent pixel.

### 1. Navigation and Viewing

The main goal is to find an empty, uncolored pixel on the grid.

| Action | Desktop (PC/Mac) | Mobile (Touchscreen) |
| :--- | :--- | :--- |
| **Zoom In/Out** | Use the **scroll wheel** on your mouse, or click the **'+' / '−'** buttons. | Use **two fingers (pinch-to-zoom)** gesture. |
| **Pan/Move Canvas** | **Click and hold the left mouse button** anywhere on the canvas, then drag the view. | **Touch and drag** with a single finger. |
| **Reset View** | Click the **'⟲'** button in the bottom right corner. | Click the **'⟲'** button in the bottom right corner. |

### 2. Selecting a Pixel

To begin coloring, you must select an empty, uncolored pixel.

| Action | Desktop (PC/Mac) | Mobile (Touchscreen) |
| :--- | :--- | :--- |
| **Select Pixel** | **Click once** on an empty white pixel. | **Tap and hold** (a brief long-press) on an empty white pixel. |
| **Status Check** | If you click an already colored pixel, a notification will appear: "This pixel is already colored!" | |

### 3. Choosing and Applying Color

Once a pixel is selected, the **Color Picker Modal** will appear, displaying the coordinates of your selected spot.

1.  **Select Color:** Choose one of the preset color options or use the custom color input to select a specific HEX code.
2.  **Apply Color:** Click the **"Apply color"** button.

### 4. Ad Requirement and Final Placement

To finalize your placement, you must view the short ad to secure the server resources required for saving your data.

1.  **Ad Start:** After clicking "Apply color," the **Video Overlay** will appear, and the ad video will attempt to **autoplay** (muted by default).
2.  **PC Playback Fix:** If the video stops or appears black (due to strict browser policies), a notification will prompt you to **click the black area** to manually resume playback.
3.  **Completion:** Once the ad is complete (or the 5-second fail-safe is triggered), the **Close Button (✕)** will appear.
4.  **Finalize:** Click the **Close Button (✕)**. Your chosen color and coordinates will be sent to the Sliz® backend, and a "Pixel drawn successfully!" notification will confirm your contribution.

---

## 👨‍💻 Backend Integration

The project relies on a Cloudflare Worker for persistent data storage:

* **Data Structure:** Pixels are stored by their key format: `X-Y` (e.g., `150-420`).
* **API Endpoints:**
    * `GET /pixels`: Retrieves the entire canvas data (color map).
    * `POST /pixel`: Saves a new pixel entry after ad validation.

---

## 🚫 Copyright and Intellectual Property Notice

**© 2025 Sliz® - All Rights Reserved.**

This project, **DrawPix**, including its core architecture, user interface, functionality logic, backend worker integration (as referenced by `WORKER_URL`), and design assets, is the exclusive intellectual property of **Sliz®**.

The code provided here is a working demonstration of the frontend functionality and is protected by **Sliz® Protected Rights License**.

**Unauthorized copying, reproduction, distribution, reverse engineering, or modification of this source code and its associated assets is strictly prohibited.** Any attempt to bypass the ad-watching mechanism, the core monetization and resource protection feature, is a direct violation of the protected rights.

---

**Thank you for contributing to the collective art of DrawPix!**
