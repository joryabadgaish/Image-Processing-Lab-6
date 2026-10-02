# Image-Processing-Lab-6

Image filtering in the frequency domain with NumPy's FFT, using the `cameraman` image.

Filtering is done by multiplying the image's FFT by a filter and inverse-transforming: `ifft2(fft2(image) * H)`.

## Tasks

- **Laplacian:** built from its closed form `H(u, v) = -4π²(u² + v²)`.
- **Sobel (X and Y):** each 3×3 kernel is padded to image size, `ifftshift`ed, and FFT'd to get its frequency response. Results match spatial convolution, and the gradient magnitude combines both directions.

## Run

```bash
pip install numpy matplotlib scikit-image scipy jupyter
jupyter notebook Lab6_Frequency_Domain_solved.ipynb
```
