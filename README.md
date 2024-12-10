# **Invisible Blue Cloak**

This project demonstrates a fun and engaging computer vision application that uses **OpenCV** to make objects or areas of a specific color (blue in this case) "invisible" by replacing them with a captured background. The program creates a magical effect similar to an **invisibility cloak**, inspired by the concept of chroma keying used in video production.

## **Features**
- Detects areas in the video feed with a specific color (blue) using the **HSV color space**.
- Replaces the detected color region with a pre-captured background, making the area appear "invisible."
- Provides real-time video processing using OpenCV.
- Optimized for smooth and interactive performance.

## **How It Works**
1. The background is captured for a few seconds at the start to create a stable reference.
2. The program converts the live video feed to the **HSV color space** for better color detection.
3. A color mask is applied to detect the specified color range (blue in this case).
4. The detected blue regions are replaced with the pre-captured background, creating an "invisible" effect.
5. The rest of the video feed remains unchanged, combining real-time interaction and augmented visuals.

## **Setup Instructions**
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/invisible-blue-cloak.git
   cd invisible-blue-cloak
   ```
2. Install the required dependencies:
   ```bash
   pip install opencv-python numpy
   ```
3. Run the program:
   ```bash
   python invisible_blue_cloak.ipynb
   ```

## **Requirements**
- Python 3.9
- Libraries: OpenCV, NumPy
- A working webcam or video feed.

## **Usage**
1. Ensure a stable background before starting the program.
2. Place an object or wear clothes that are primarily blue in color.
3. Watch as the blue areas become invisible, replaced by the captured background!

## **Customizations**
- Modify the `lower_blue` and `upper_blue` ranges in HSV to target a different color.
- Adjust the `iterations` for morphological operations (`morphologyEx` and `dilate`) to refine the mask.

## **Demo**
https://github.com/user-attachments/assets/ce38d446-062d-44b5-9ce8-e4259e0b7faa


## **Contributing**
Contributions are welcome! Feel free to open issues or submit pull requests to enhance the project.
