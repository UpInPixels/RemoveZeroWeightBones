# Remove Zero Weight Bones [![Add to VCC](https://img.shields.io/badge/VCC-Add%20to%20VCC-36a64f?style=for-the-badge&logo=vrchat&logoColor=white)](https://upinpixels.github.io/UpInPixels-Utilities/)

An Editor utility for Unity that cleans up unused zero-weight bone GameObjects from your avatar or model hierarchy.

It checks all **Skinned Mesh Renderers** bound to the assigned armature and safely deletes unweighted bones (bottom-up) while explicitly keeping parent transforms, root bones, and active mesh renderers intact.

---

## Features

* **Zero Weight Hierarchy Cleanup:** Detects and deletes bone transforms that have zero mesh vertex weights assigned across all associated SkinnedMeshRenderers.
* **Twist Bone Protection:** Built-in option to automatically preserve twist bones (bones with `twist` in the name or starting with `_`) and their parent chains.
* **Safe Deletion:**
* Deletes child bones first (depth-sorted) to preserve hierarchy integrity.
* Automatically skips objects containing **Renderers** or **Colliders**.
* Includes options to safeguard or remove bones containing extra components (e.g., PhysBones).


* **Undo Support:** All deletions are integrated into Unity's Undo system (`Ctrl + Z` / `Cmd + Z`).
* **In-Editor Logging:** Built-in summary counter and detailed log window directly inside the Editor GUI.

---

## Installation

### Option 1: Via VRChat Companion App (VCC)

[![Add to VCC](https://img.shields.io/badge/VCC-Add%20to%20VCC-36a64f?style=for-the-badge&logo=vrchat&logoColor=white)](https://upinpixels.github.io/UpInPixels-Utilities/)

or

1. Open **VRChat Companion App (VCC)**.
2. Go to **Settings** -> **Packages** -> **Add Repository**.
3. Paste the VCC listing URL:
`[https://UpInPixels.github.io/UpInPixels-Utilities/index.json](https://UpInPixels.github.io/UpInPixels-Utilities/index.json)`
4. Add **Remove Zero Weight Bones** to your VCC project.

---

### Option 2: Unity Package Manager (Git URL)

1. Open your Unity project.
2. Go to **Window > Package Manager**.
3. Click the **`+`** icon in the top-left corner -> **Add package from git URL...**.
4. Enter:
`[https://github.com/UpInPixels/RemoveZeroWeightBones.git?path=/Packages/com.upinpixels.removezeroweightbones](https://github.com/UpInPixels/RemoveZeroWeightBones.git?path=/Packages/com.upinpixels.removezeroweightbones)`

---

## Usage

1. Open the tool from the top menu bar:
**`Tools > UpInPixels > Remove Zero Weight Bones`**
2. Assign your armature object to the **Armature Root** field *(select the `Armature` root bone transform, not the main avatar root object)*.
3. Configure your options:
* **Keep Twist Bones:** Prevents deletion of twist bones (`*twist*` or starting with `_`).
* **Delete Empty Parent Bones:** Allows deletion of zero-weight bones that carry extra components (like PhysBones) once their children are removed.


4. Click **Remove Zero Weight Bones**.

---

## Requirements

* **Unity Version:** 2019.4 / 2021.3 / 2022.3 or newer
* **Module:** Unity Editor (Editor script only)

---

## Author

Developed by **UpInPixels** (Uppy)

* **Store:** [Payhip](https://payhip.com/upinpixels)
* **Main Repo:** [UpInPixels-Utilities](https://www.google.com/search?q=https://github.com/UpInPixels/UpInPixels-Utilities)