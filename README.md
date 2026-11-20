# Image Segmentation with Thresholding: Global, Adaptive & Otsu

![Python 3](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![Course · CV](https://img.shields.io/badge/Course%20%C2%B7%20CV-2563EB?style=flat-square)

From-scratch implementations and comparison of three classical image-segmentation thresholding
methods on grayscale images, following the formulations in Gonzalez & Woods' *Digital Image Processing*:

1. **Basic global thresholding** — iteratively refines an initial threshold (the image's mean gray level)
   by splitting pixels into two groups and re-averaging until the threshold converges.
2. **Adaptive (local) thresholding** — computes a per-pixel threshold from local window statistics
   (local mean and local standard deviation over a `k×k` neighborhood), handling non-uniform illumination
   that a single global threshold cannot.
3. **Otsu's method** — finds the optimal global threshold by maximizing between-class variance
   across all 256 gray levels.

## Repository Structure

| File | Description |
|---|---|
| `global_adaptive_otsu_aio_final.ipynb` | All three methods implemented and visualized step by step |
| `Bao_Cao_ThiGiacMayTinh.docx` | Course report (Vietnamese) |
| `Thị giác máy tính.pptx` | Slides (Vietnamese) |

## Requirements

- Python 3
- `opencv-python`, `numpy`, `matplotlib`

Run the notebook with Jupyter:

```bash
jupyter notebook global_adaptive_otsu_aio_final.ipynb
```

> Course project — Computer Vision (CV)
