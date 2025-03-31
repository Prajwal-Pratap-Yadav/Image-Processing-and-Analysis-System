# Image Processing and Analysis System

## Overview
This project implements an image processing pipeline using MATLAB to analyze and manipulate digital images. The system performs operations such as noise reduction, edge detection, segmentation, and frequency-domain analysis, providing a practical framework for understanding key image processing concepts.

## Features
- Image acquisition and grayscale conversion
- Noise removal using Gaussian filtering
- Edge detection using the Canny algorithm
- Image segmentation using thresholding (Otsu’s method)
- Object analysis with region properties
- Contrast enhancement using histogram equalization
- Morphological operations (erosion and dilation)
- Fourier transform for frequency analysis
- Laplacian edge detection for intensity transitions

## Technologies Used
- **Programming Language:** MATLAB
- **Software Requirements:** MATLAB with Image Processing Toolbox
- **Hardware Requirements:** Standard computer (Minimum: 4GB RAM, i3 Processor)
- **Supported Image Formats:** JPEG, PNG

## Installation
1. Install MATLAB and ensure the Image Processing Toolbox is available.
2. Clone this repository:
   ```sh
   git clone https://github.com/yourusername/Image-Processing-and-Analysis-System.git
   ```
3. Open MATLAB and navigate to the project directory.

## Usage
1. **Load an image:**
   ```matlab
   img = imread('sample.jpg');
   ```
2. **Convert to grayscale:**
   ```matlab
   gray_img = rgb2gray(img);
   ```
3. **Apply Gaussian filtering:**
   ```matlab
   filtered_img = imgaussfilt(gray_img, 2);
   ```
4. **Perform edge detection:**
   ```matlab
   edge_img = edge(filtered_img, 'Canny');
   ```
5. **Segment the image using thresholding:**
   ```matlab
   bw_img = imbinarize(filtered_img);
   ```
6. **Save processed images:**
   ```matlab
   imwrite(edge_img, 'processed_image.jpg');
   ```

## Example Output
The project generates a series of images demonstrating different processing stages:
1. **Original Image** - Raw input image
2. **Grayscale Image** - Converted from RGB to grayscale
3. **Filtered Image** - Smoothed using Gaussian filter
4. **Edge Detection** - Processed using Canny edge detection
5. **Segmented Image** - Binary thresholding applied
6. **Contrast Enhanced Image** - Histogram equalization
7. **Eroded and Dilated Images** - Morphological operations
8. **Frequency Domain Representation** - Fourier Transform applied
9. **Laplacian Edge Detection** - Highlighted intensity transitions

## Results and Conclusion
The project successfully implements multiple image processing techniques for analysis and enhancement. The techniques demonstrated can be applied in medical imaging, remote sensing, industrial automation, and AI-based vision systems. Future improvements may include:
- Integration of adaptive thresholding methods
- Deep learning-based feature extraction
- Real-time video processing for advanced applications

## Contributors
- **Prajwal Pratap Yadav**
- **Ashish Kumar Yadav**
- **Pratham Chaturvedi**

## License
This project is open-source and available under the [MIT License](LICENSE).
