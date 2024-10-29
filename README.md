# Introduction to Image Processing
Image processing involves manipulating digital images through algorithms, with applications in fields such as medical imaging, facial recognition, and computer vision. Techniques like blurring, edge detection, and transformations can help emphasize or isolate features within an image, making it easier to analyze or recognize patterns.
# Original image

![M2](https://github.com/user-attachments/assets/c5bfcc8f-85cf-4cd4-8fc9-0b342c7bbd58)

## Filters and Techniques

## Gaussian Blur
Gaussian Blur is a low-pass filter that smooths an image by reducing noise and details. It uses a Gaussian function to calculate the transformation on pixel intensity, creating a blur effect. It is commonly used as a preprocessing step for edge detection.

## Parameters:
**ksize:** Size of the kernel (usually odd).<br>
**sigmaX:** Standard deviation in the X direction.<br>

![MA](https://github.com/user-attachments/assets/cdd99cad-78d7-464a-a6a6-13a0a77b4486)

## Gabor Filter
The Gabor filter captures texture information in an image by applying a sinusoidal wave modulated by a Gaussian envelope. This filter is particularly useful for feature extraction and texture analysis, commonly used in image recognition.

## Parameters:
**ksize:** Size of the kernel.<br>
**sigma:** Standard deviation of the Gaussian envelope.<br>
**lambd:** Wavelength of the sinusoidal component.<br>
**gamma:** Spatial aspect ratio.<br>
**theta:** Orientation (angle) of the filter.<br>

![download](https://github.com/user-attachments/assets/f1cec897-7518-4368-a425-5909b4d7f1a1)

## Laplacian Edge Detection
The Laplacian filter is a high-pass filter used for edge detection by calculating the second derivative of the image intensity. It is particularly sensitive to regions with rapid intensity changes, helping to highlight edges.

## Parameters:
**ksize:** Size of the filter kernel.<br>

![download (1)](https://github.com/user-attachments/assets/6125fb84-84e8-47b9-8b24-aca28100d49b)

# Sobel Edge Detection
Sobel Edge Detection calculates the gradient of the image intensity in both X and Y directions. It is often used to find the edges of objects in images by highlighting areas with high gradient magnitudes. The Sobel filter can be applied individually in X and Y directions and then combined to obtain the full edge map.

## Parameters:
**ksize:** Size of the Sobel kernel.<br>
**dx, dy:** Order of derivative in X and Y directions, respectively.

![MB](https://github.com/user-attachments/assets/0bfce881-b0fc-4583-bc45-81dd7a1eafc0)

# Fourier Transform
The Fourier Transform converts an image from the spatial domain to the frequency domain, allowing analysis of the image's frequency components. In the frequency domain, high-frequency components correspond to edges and fine details, while low frequencies represent the overall structure of the image. The magnitude spectrum of the Fourier Transform can be visualized to reveal the dominant frequencies.

![download (3)](https://github.com/user-attachments/assets/6f9a439f-d753-4267-a175-07df081ee457)

# Canny Edge Detection
Canny Edge Detection is a multi-step algorithm for detecting edges. It uses gradient-based edge detection followed by Non-Maximum Suppression to thin out the edges, resulting in cleaner edge detection. Canny Edge Detection is widely used for detecting objects and edges in images.

## Parameters:
**threshold1, threshold2:** Lower and upper thresholds for edge detection.

![download (4)](https://github.com/user-attachments/assets/0ce3eb1c-48bf-4fd0-8001-e19e2c13b20c)

# Installation
To use this project, you need to have Python and OpenCV installed.

`pip install opencv-python numpy matplotlib`

# Examples
## Below are examples of the filters applied to an example image:

**Gaussian Blur** - Smooths the image by reducing noise.<br>
**Gabor Filter** - Extracts texture information, showing various angles.<br>
**Laplacian Edge Detection** - Highlights regions of rapid intensity change.<br>
**Sobel Edge Detection** - Computes edges in the X and Y directions.<br>
**Fourier Transform** - Shows the frequency spectrum of the image.<br>
**Canny Edge Detection** - Detects strong edges with Non-Maximum Suppression.<br>

Each filter demonstrates how specific image features can be extracted and visualized, helping in applications such as object detection, image enhancement, and computer vision tasks.
