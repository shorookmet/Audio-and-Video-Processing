# Audio and Video Processing

## Overview

This project demonstrates video frame extraction, color space conversion, and block-based motion analysis using Python. The workflow includes:
- Extracting frames from a video file
- Converting frames to the YCrCb color space
- Dividing frames into blocks and performing block matching
- Calculating residuals for motion estimation

## Features

- Loads video files and extracts all frames
- Converts frames from RGB to YCrCb color space
- Splits frames into 8x8 blocks (with and without overlap)
- Implements block matching using Sum of Absolute Differences (SAD)
- Computes residual blocks for motion analysis
- Visualizes frames and block results

## Requirements

- Python 3.x
- OpenCV (`cv2`)
- NumPy
- Google Colab (for `google.colab` and `cv2_imshow`)

Install dependencies with:
```bash
pip install opencv-python numpy
```
> **Note:** Some code is designed for Google Colab (e.g., mounting Google Drive, `cv2_imshow`). For local use, adapt these parts as needed.

## Data Structure

- Expects a video file (e.g., `car_co.mp4`) in your Google Drive or local path.

## Usage

1. **Extract Frames from Video**
   - The notebook loads a video and extracts all frames into a list.

2. **Convert to YCrCb**
   - Each frame is converted from RGB to YCrCb color space.

3. **Block Processing**
   - Frames are divided into 8x8 blocks (with and without overlap).
   - Block matching is performed between consecutive frames using SAD.
   - Residuals are computed for motion analysis.

4. **Visualization**
   - Frames and block results can be visualized using `cv2_imshow`.

## Example

To run the workflow, execute the notebook cells in order.  
Make sure to update the video file path as needed.

## Customization

- Adjust block size or overlap in the provided functions.
- Modify the video path to use your own video files.

## Acknowledgements

- OpenCV, NumPy, and Google Colab for their open-source tools.
