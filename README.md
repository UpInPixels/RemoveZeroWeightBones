# Remove Zero Weight Bones

An editor utility tool for Unity and VRChat avatars that cleans up unused skinning bones with zero weights. Optimizes avatar performance, reduces hierarchy clutter, and improves project maintainability.

---

## 🚀 Installation

### Option 1: Via VRChat Companion App (VCC) — Recommended

1. Open **VRChat Companion App (VCC)**.
2. Go to **Settings** -> **Packages** -> **Add Repository**.
3. Enter the listing URL:
`[https://UpInPixels.github.io/UpInPixels-Utilities/index.json](https://UpInPixels.github.io/UpInPixels-Utilities/index.json)`
4. Find **Remove Zero Weight Bones** in your project package list and click **Add**.

---

### Option 2: Manual Installation (Unity Package Manager)

1. In Unity, open **Window > Package Manager**.
2. Click the **`+`** icon in the top left corner and select **Add package from git URL...**.
3. Enter the HTTPS repository URL:
`[https://github.com/UpInPixels/RemoveZeroWeightBones.git?path=/Packages/com.upinpixels.removezeroweightbones](https://github.com/UpInPixels/RemoveZeroWeightBones.git?path=/Packages/com.upinpixels.removezeroweightbones)`

---

## 🛠️ Features

* 🧹 **Automatic Scanning:** Scans Skinned Mesh Renderers on your selected avatar/model for bones assigned 0 weight across all vertices.
* ⚡ **Optimization:** Safely strips unused bone transforms from the avatar hierarchy and mesh bindposes.
* 🔒 **Safe Mode:** Preserves crucial root bones, human body bones, and custom-flagged dynamic bones/constraints.
* 📑 **Clean Logging:** Displays a clear log in the Unity Console highlighting removed bones and performance improvements.

---

## 📖 Usage Guide

1. Select your Avatar or Model root object in the Unity Hierarchy.
2. Navigate to **`Tools > UpInPixels > Remove Zero Weight Bones`** in the top menu bar.
3. Review the detected zero-weight bones in the preview window.
4. Click **`Process & Clean Bones`**.

---

## 🔧 Requirements

* **Unity Version:** 2022.3.x or newer (compatible with Unity 2019/2021)
* **VRChat SDK:** VRChat SDK3 (Avatars) *[Optional]*

---

## 👤 Author & Support

* **Author:** Uppy ([UpInPixels](https://payhip.com/upinpixels))
* **Utilities Repo:** [UpInPixels-Utilities](https://www.google.com/search?q=https://github.com/UpInPixels/UpInPixels-Utilities)
* **Issues / Feedback:** Open an issue on the [GitHub Repository](https://www.google.com/search?q=https://github.com/UpInPixels/RemoveZeroWeightBones/issues).