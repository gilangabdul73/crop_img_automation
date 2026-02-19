# Batch Portrait Cropper (3x4 Dimension)

This tool automates the process of cropping a large collection of portrait images into the standard **3:4 aspect ratio**. It is optimized for Google Colab and handles batch processing of JPG and PNG files.

## Features
* **Batch Processing:** Automatically loops through folders (e.g., `day_1`).
* **Smart Cropping:** Maintains a 3:4 ratio regardless of the original image dimensions.
* **Adjustable Focus:** Custom `focus_point_y` parameter to ensure the subject's face is correctly positioned (default set to `0.15` for head-centered crops).
* **Automatic Cleaning:** Removes "Copy of " prefixes from filenames during the output process.
* **Quality Control:** Saves JPEGs at 100% quality and optimizes PNG files.

## Parameters
* `zoom_factor`: Controls how "close" the crop is (0.9 = 90% of the maximum possible crop area).
* `focus_point_x`: Horizontal alignment (0.5 for center).
* `focus_point_y`: Vertical alignment (lower values move the crop window higher).

## Requirements
* Python 3.x
* Pillow (PIL)
* Google Colab (for Drive mounting)
