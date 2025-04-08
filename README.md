# Image Resizer and Compressor

A simple, client-side tool for **bulk image resizing** and **file-size compression**. Drag & drop images or browse from your computer, set max width/height, and choose a target file size. Includes **individual** and **batch** renaming (disallows name collisions) and a single ZIP export.

## Features

- **Drag & Drop** support: Quickly add images by dragging them onto the page.
- **Browse** button for single/multiple file selection, or entire folder import.
- **Resize** images to a specified max width/height (keeps aspect ratio).
- **Compress** images (exported as **JPEG**) to meet a target file size (using a binary search on JPEG quality).
- **Remove** button for each selected file to easily manage your list.
- **Rename** options:
  - **Individual rename** for each compressed image (prompts you to enter a new name).
  - **Batch rename** (all images get `prefix-1.jpg`, `prefix-2.jpg`, etc.) – collisions are disallowed.
- **Export**: Download results individually or export them all at once as a single `.zip`.
- Displays an **error** if minimal quality still can’t meet your target file size (i.e., “Could not reach target size at minimal quality.”)

## How It Works

1. **Load images**: Drag & drop or use the “Browse Files” / “Browse Folder” buttons.
2. **Set parameters** (optional): 
   - `Max Width` / `Max Height` (use `0` to ignore that dimension).  
   - `Target Size (KB)` for final output.
3. **Resize & Compress**:
   - The script resizes images (if needed) to respect your width/height.
   - It then uses a **binary search** on JPEG quality to approximate your target file size.
4. **Preview & Rename**:
   - Each result shows a final preview, approximate size, and a “Download” link.
   - Rename individually or apply a **batch prefix** rename. No duplicate file names allowed.
5. **Export**: Optionally download each file or **Export All (ZIP)**.

## Quick Start

1. **Clone or download** this repository.
2. **Open** `index.html` in a modern browser (Chrome, Firefox, Edge, Safari, etc.).
3. **Add images** (drag & drop or browse).
4. **Adjust** `Max Width`, `Max Height`, and `Target Size (KB)` as needed.
5. Click **“Resize & Compress”**.
6. **Rename** (if desired) either individually or via **batch rename** prefix.
7. **Export** results as a single `.zip` or download individually.

## Minimal Requirements

- **No installation** needed; everything runs client-side.
- Just ensure your browser supports HTML5 `<canvas>`, drag/drop, and ES6+ JavaScript features.

## Screenshots

![Screenshot 2025-03-18 at 9 50 13 AM](https://github.com/user-attachments/assets/76870e44-7ce5-46ac-b1f8-eb18abd818bb)
![Screenshot 2025-03-18 at 9 50 32 AM](https://github.com/user-attachments/assets/90eb8fde-1864-4c20-9dd4-ed515e8bbab5)
![Screenshot 2025-03-18 at 9 51 19 AM](https://github.com/user-attachments/assets/9c84c7c0-2a51-4468-b19a-c890f32f4760)
