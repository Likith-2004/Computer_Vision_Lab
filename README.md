Introduction to Image Processing
Image processing involves manipulating digital images through algorithms, with applications in fields such as medical imaging, facial recognition, and computer vision. Techniques like blurring, edge detection, and transformations can help emphasize or isolate features within an image, making it easier to analyze or recognize patterns.

Filters and Techniques
1. Gaussian Blur
Gaussian Blur is a low-pass filter that smooths an image by reducing noise and details. It uses a Gaussian function to calculate the transformation on pixel intensity, creating a blur effect. It is commonly used as a preprocessing step for edge detection.

Parameters:
ksize: Size of the kernel (usually odd).
sigmaX: Standard deviation in the X direction.
2. Gabor Filter
The Gabor filter captures texture information in an image by applying a sinusoidal wave modulated by a Gaussian envelope. This filter is particularly useful for feature extraction and texture analysis, commonly used in image recognition.

Parameters:
ksize: Size of the kernel.
sigma: Standard deviation of the Gaussian envelope.
lambd: Wavelength of the sinusoidal component.
gamma: Spatial aspect ratio.
theta: Orientation (angle) of the filter.
3. Laplacian Edge Detection
The Laplacian filter is a high-pass filter used for edge detection by calculating the second derivative of the image intensity. It is particularly sensitive to regions with rapid intensity changes, helping to highlight edges.

Parameters:
ksize: Size of the filter kernel.
4. Sobel Edge Detection
Sobel Edge Detection calculates the gradient of the image intensity in both X and Y directions. It is often used to find the edges of objects in images by highlighting areas with high gradient magnitudes. The Sobel filter can be applied individually in X and Y directions and then combined to obtain the full edge map.

Parameters:
ksize: Size of the Sobel kernel.
dx, dy: Order of derivative in X and Y directions, respectively.
5. Fourier Transform
The Fourier Transform converts an image from the spatial domain to the frequency domain, allowing analysis of the image's frequency components. In the frequency domain, high-frequency components correspond to edges and fine details, while low frequencies represent the overall structure of the image. The magnitude spectrum of the Fourier Transform can be visualized to reveal the dominant frequencies.

6. Canny Edge Detection
Canny Edge Detection is a multi-step algorithm for detecting edges. It uses gradient-based edge detection followed by Non-Maximum Suppression to thin out the edges, resulting in cleaner edge detection. Canny Edge Detection is widely used for detecting objects and edges in images.

Parameters:
threshold1, threshold2: Lower and upper thresholds for edge detection.
Installation
To use this project, you need to have Python and OpenCV installed.

Examples
Below are examples of the filters applied to an example image:

Gaussian Blur - Smooths the image by reducing noise.
Gabor Filter - Extracts texture information, showing various angles.
Laplacian Edge Detection - Highlights regions of rapid intensity change.
Sobel Edge Detection - Computes edges in the X and Y directions.
Fourier Transform - Shows the frequency spectrum of the image.
Canny Edge Detection - Detects strong edges with Non-Maximum Suppression.
Each filter demonstrates how specific image features can be extracted and visualized, helping in applications such as object detection, image enhancement, and computer vision tasks.

