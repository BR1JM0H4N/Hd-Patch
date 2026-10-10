<div align="center">
  <img src="logo.png" alt="HD Patch Logo" width="160" height="160">
  <h1>HD Patch</h1>
  <p><b>Put your HD original back into an outpainted image — seamlessly and locally.</b></p>

  <p>
    <a href="https://capacitorjs.com"><img src="https://img.shields.io/badge/capacitor-1194F6?style=flat&logo=capacitor&logoColor=white" alt="Capacitor Badge"></a>
    <a href="https://developer.android.com"><img src="https://img.shields.io/badge/Android-3DDC84?style=flat&logo=android&logoColor=white" alt="Android Badge"></a>
    <a href="https://developer.mozilla.org/en-US/docs/Web/Progressive_Web_Apps"><img src="https://img.shields.io/badge/PWA-5A0FC8?style=flat&logo=pwa&logoColor=white" alt="PWA Badge"></a>
    <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License Badge">
    <img src="https://img.shields.io/badge/client--side-privacy-green.svg" alt="Privacy First">
  </p>
</div>

---

## 🌟 What is HD Patch?

AI outpainting tools (such as Generative Fill, Stable Diffusion outpainting, and others) excel at expanding the boundaries of your photos, but they typically output downscaled, compressed low-resolution pictures. 

**HD Patch** solves this problem instantly. Simply drop in your low-res outpainted picture and your crisp original HD photo, and HD Patch will:
1. Automatically find where the original belongs using sub-pixel Normalized Cross-Correlation (NCC).
2. Precisely stretch and align the image matrices.
3. Seamlessly blend the sharp original pixels back into the outpainted canvas with adjustable edge feathering and local color correction.

Everything runs entirely client-side in your web browser with zero server uploads, keeping your images 100% private.

---

## ✨ Features

- **⚡ Auto-Align Engine:** Multi-scale template matching calculates exact position, rotation scale, and sub-pixel registration automatically.
- **👁️ Multiple View Modes:** Toggle effortlessly between **Overlay** (with adjustable opacity), **Difference** (darkness indicates a pixel-perfect match), and **Result** preview.
- **🎛️ Fine Controls:** Nudge buttons with adjustable steps ($4\text{px}$, $1\text{px}$, $0.2\text{px}$) and fine scale adjustments ($\pm0.1\%$, $\pm1\%$).
- **🎨 Smart Blending & Color Matching:** Customizable edge feathering and low-frequency color correction to eliminate harsh seams between the original and outpainted sections.
- **📐 Flexible Export Options:** Export at Native HD proportions, 4K, or 8K resolutions.
- **🔒 Privacy First:** 100% browser-based processing using canvas and Web APIs. No data ever leaves your device.
- **📱 PWA & Android Ready:** Fully responsive design built to run natively on mobile via [Capacitor](https://capacitorjs.com).

---

## 📱 Mobile App Integration (Capacitor & Android)

HD Patch is structured as a Progressive Web App (PWA), making it trivial to package into a native Android application using **Ionic Capacitor**. 

### Quick Android Build Steps:
1. Initialize Capacitor in your project:
   ```bash
   npm init -y
   npm install @capacitor/core @capacitor/cli
   npx cap init
   ```
2. Add the Android platform:
   ```bash
   npm install @capacitor/android
   npx cap add android
   ```
3. Open and run the project in Android Studio:
   ```bash
   npx cap open android
   ```

---

## 🚀 Usage Guide

1. **Upload Images:** 
   - Drop your low-resolution **Outpainted Image** into the first picker.
   - Drop your sharp, unscaled **HD Original** into the second picker.
2. **Align:** 
   - Click **Auto-align** to let the app locate the original automatically, or drag and pinch/scroll to place it manually.
   - Switch to **Difference View** to check alignment (a true match results in deep black). Use the nudge buttons or keyboard arrows for microscopic adjustments.
3. **Blend & Export:**
   - Adjust edge feathering and color matching to blend the seams smoothly.
   - Choose your preferred output resolution (Native, 4K, or 8K).
   - Click **Create PNG** followed by **Save PNG** to download your high-resolution restored masterpiece.

---

## 🛠️ Tech Stack

- **HTML5 / CSS3 / JavaScript (ESModules):** Zero heavy frameworks required; lightweight, high-performance vanilla implementation.
- **HTML5 Canvas API:** High-performance image manipulation, transformation matrices, and multi-scale image pyramids.
- **Progressive Web App (PWA):** Installable directly on desktop and mobile devices.
- **Ionic Capacitor:** Seamless bridge for publishing as a native Android application.

---

## 🤝 Contributing

Contributions, bug reports, and feature requests are warmly welcomed! 
1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the Branch (`git origin push feature/AmazingFeature`).
5. Open a Pull Request.

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.