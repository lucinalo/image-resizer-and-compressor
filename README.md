# Image Resizer and Compressor

A simple, client-side tool for bulk image resizing and file-size compression. Drag & drop images or browse from your computer, set max width/height, and choose a target file size.

## Features

- **Drag & Drop** support: Quickly add images by dragging them onto the page.
- **Browse** button for file selection.
- **Optionally resize** images to a specified max width/height (keeping aspect ratio).
- **Compress** images (JPEG) to meet a target file size (where possible).
- **Numbered list** of selected files and an easy **Remove** button for each file.
- Results include final preview, file size, and a direct **Download** link.

## How It Works

1. **Load images** via drag & drop or the Browse button.
2. **Optional resize**: Set desired `Max Width` or `Max Height` (leave as `0` to ignore).
3. **Compress**: The script uses a binary search on JPEG quality to aim for your target file size (in KB).
4. **Preview**: See the final image’s approximate size and a download link.

## Quick Start

1. **Open** `index.html` in your browser.
2. **Drag & drop** or **Browse** for images.
3. Adjust `Max Width`, `Max Height`, `Target Size (KB)` if you want.
4. Click **Resize & Compress** to process them.
5. Download the results from the displayed previews.

## Installation

No installation needed—purely client-side:

- Clone or download this repository.
- Open `index.html` in any modern browser.

![Screenshot 2025-03-18 at 9 50 13 AM](https://github.com/user-attachments/assets/76870e44-7ce5-46ac-b1f8-eb18abd818bb)
![Screenshot 2025-03-18 at 9 50 32 AM](https://github.com/user-attachments/assets/90eb8fde-1864-4c20-9dd4-ed515e8bbab5)
![Screenshot 2025-03-18 at 9 51 19 AM](https://github.com/user-attachments/assets/9c84c7c0-2a51-4468-b19a-c890f32f4760)
