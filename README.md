# Image-Processing-Laplacian-spatial-
Spatial Domain Laplacian Filtering: Convolve image with Laplacian kernel to enhance edges and details.  Frequency Domain Laplacian Filtering: Apply Fourier Transform, multiply with Laplacian filter, and inverse transform to achieve similar enhancement via frequency manipulation.

Laplacian Image Filtering in Spatial Domain:

1. Input Image: Begin with the original image.
2. Kernel Construction: Create a Laplacian kernel (e.g., [[0, 1, 0], [1, -4, 1], [0, 1, 0]]) that represents the second derivative of the image.
3. Convolution: Slide the Laplacian kernel over the image and compute the element-wise multiplication followed by summation of pixel values at each position. This results in a filtered image.
4. Normalization: Depending on the kernel used, you might need to apply normalization to enhance the contrast in the filtered image.
5. Display: Display the original image and the Laplacian-filtered image to observe the edges and details emphasized by the filter.


Laplacian Image Filtering in Frequency Domain:

1. Input Image: Start with the original image.
2. Fourier Transform: Compute the 2D Fourier Transform of the image to convert it into the frequency domain.
3. Filter Creation: Create a filter in the frequency domain that corresponds to the Laplacian operation. This is done by constructing a matrix that represents the Laplacian kernel.
4. Frequency Domain Multiplication: Multiply the Fourier-transformed image with the Laplacian filter in the frequency domain using element-wise multiplication.
5. Inverse Fourier Transform: Apply the inverse Fourier Transform to the product obtained in the previous step to bring the image back to the spatial domain.
6. Display: Display the original image and the Laplacian-filtered image to observe the edges and details emphasized by the filter.

Both approaches aim to emphasize the edges and fine details in an image. The spatial domain approach uses direct convolution, while the frequency domain approach takes advantage of the convolution theorem to perform filtering in the frequency domain using Fourier Transforms. The choice between the two methods often depends on computational efficiency and the desired level of control over the filtering process.
