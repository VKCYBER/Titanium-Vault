# Titanium-Vault
​🧬 ChanForge v23: Neural Nexus

> **The Ultimate Offline-First Hybrid AI Browser & Archivist for Android.**

![Android](https://img.shields.io/badge/Platform-Android-green?logo=android)
![Java](https://img.shields.io/badge/Language-Java_%7C_HTML5-orange?logo=java)
![AI](https://img.shields.io/badge/AI-TensorFlow_%7C_WebLLM-blue)
![Offline](https://img.shields.io/badge/Status-Offline_Ready-purple)

## 📖 Overview

**ChanForge v23 (Codename: Neural Nexus)** is an experimental Android application that bridges the gap between the web and native hardware. It is designed to be a completely self-contained ecosystem that "learns" from the internet when online and remains fully functional when offline.

It utilizes a **Hybrid Architecture**: A high-performance Native Java Core handles heavy background tasks (archiving, hardware acceleration, file I/O), while a modern HTML5/JS Neural Interface manages the AI interactions, RAG (Retrieval Augmented Generation), and local vector database.

## 🚀 Key Features

### 🧠 The Hivemind (Auto-Hybrid Learning)
* **Background Intelligence:** Uses Android `WorkManager` to wake up every 15 minutes (if online), scrape targeted web content (simulated 4chan/Reddit threads), and inject new knowledge into the local database.
* **Offline RAG:** Ask the AI questions about content you browsed days ago, even without a signal. The AI searches your local "Vault" to construct answers.

### ⚡ Neural Nexus Bridge
* **Native Upscaling:** Bypasses slow JavaScript processing by sending images to the Android Native Layer for hardware-accelerated upscaling.
    * *Current Implementation:* High-Quality Bicubic Native Scaling (Instant).
    * *Ready For:* TFLite RealESRGAN injection.
* **Haptic Feedback:** Physical vibration responses triggered by AI events.

### 🔒 The Vault (Offline Internet)
* **Zero-Latency Browsing:** All saved threads and images are stored in `IndexedDB`. The app loads in <0.1s.
* **Privacy First:** No external servers. No cloud tracking. Your data stays on your `data/data/com.chanforge` partition.

## 🛠️ Tech Stack

* **Core:** Android SDK (Java), API 26+
* **UI/Brain:** WebView Asset Loader (HTML5, TailwindCSS, FontAwesome)
* **AI Engine:** TensorFlow.js (Vision), WebLLM (Text), Android Native Bitmap (Image Processing)
* **Background:** Android WorkManager, WakeLocks
* **Storage:** Room (Java) + IndexedDB (JS) Hybrid

## 📦 Installation & Build Guide

### Prerequisites
* Android Studio Iguana or newer.
* JDK 17.
* Physical Android Device (Recommended for AI performance) or Emulator with Hardware Graphics enabled.

### Step-by-Step
1.  **Clone the Repo:**
    ```bash
    git clone [https://github.com/YourUsername/ChanForge.git](https://github.com/YourUsername/ChanForge.git)
    ```
2.  **Open in Android Studio:**
    Select the root folder. Allow Gradle to sync.
3.  **Add Assets:**
    Ensure `index.html` is placed inside `app/src/main/assets/`.
4.  **Build & Run:**
    Press the green **Run** button (Shift+F10).

## 🔮 Roadmap
* [ ] Integration of `.tflite` RealESRGAN models for true AI Super Resolution.
* [ ] Direct 4chan API Proxy switcher in Settings.
* [ ] "Deep Sleep" mode for extreme battery saving.
* [ ] Widget support for Hivemind stats.

## ⚠️ Disclaimer
This project is for educational and research purposes only. It is designed to simulate how offline AI architectures can function. The "crawling" features currently simulate data fetching for demonstration purposes. Users are responsible for any content accessed or generated.

---
*Built with code & chaos by [VKCYBER]*

