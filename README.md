# Statistical Image Analysis
### BIOE 484 · Biomedical Image Computing · UIUC · Spring 2026

A collection of interactive reference modules built alongside coursework for BIOE 484. Each file is a self-contained HTML visualization — no build step, no dependencies, just open in a browser or serve via GitHub Pages.

**Live site →** `https://frankthetank7277.github.io/statistical-image-analysis/`

---

## Modules

| # | Module | Topic | File |
|---|--------|-------|------|
| 01 | Convolution Walkthrough | Step-by-step convolution of two signals | `convolution_walkthrough.html` |
| 02 | Fourier Walkthrough | Frequency domain decomposition, animated | `fourier-walkthrough.html` |
| 03 | Image Sampling | Spatial sampling and aliasing in 2D images | `image_sampling.html` |
| 04 | Sampling Theory | Nyquist theorem and reconstruction | `sampling_theory_interactive.html` |
| 05 | Gaussian Filtering | Gaussian smoothing, DoG & LoG kernels | `gaussian_filtering_viz.html` |
| 06 | Image Transforms, Relaxation & Denoising | Geometric & intensity transforms · MRF relaxation · bilateral & TV denoising | `image_transforms_denoising.html` |
| 07 | Canny Edge Detector | Full pipeline: Gaussian → gradient → NMS → hysteresis | `canny_explorer.html` |
| 08 | Edge Detection Explorer | Canny · Sobel · Hough Transform · RANSAC · LoG | `edge_detection_explorer.html` |
| 09 | Keypoint Detection & Harris Corners | Structure tensor · Harris criterion · invariance | `keypoint-detection.html` |
| 10 | Image Filters — Derivation & Intuition | Box · Gaussian · Sobel · Prewitt · Laplacian · LoG | `image-filters-viz.html` |
| 11 | Affine Transformations | 3×3 matrix anatomy · translation · rotation · scale · shear | `affine_transform.html` |

---

## Structure

Each module is a single `.html` file with embedded CSS and JavaScript — no external dependencies beyond Google Fonts. The `index.html` at the root serves as the landing page and links to all modules.

```
statistical-image-analysis/
├── index.html                        ← landing page
├── affine_transform.html
├── canny_explorer.html
├── convolution_walkthrough.html
├── edge_detection_explorer.html
├── fourier-walkthrough.html
├── gaussian_filtering_viz.html
├── image-filters-viz.html
├── image_sampling.html
├── image_transforms_denoising.html
├── keypoint-detection.html
├── sampling_theory_interactive.html
└── README.md
```

---

## Design

All modules follow a shared dark-theme design system — `DM Sans` + `DM Mono` + `Bebas Neue`, deep navy backgrounds, blue/cyan accents. Built to be readable on a laptop during a study session.

---

## Adding a new module

1. Build the visualization as a single `.html` file
2. Drop it in the repo root
3. Add an entry to the `<ul id="filelist">` in `index.html` — the module count updates automatically

```html
<li class="module-item" style="--item-color: #YOUR_COLOR">
  <a href="your_file.html">
    <div class="module-left">
      <span class="module-index">NN</span>
      <div class="module-info">
        <div class="module-name">Module Name</div>
        <div class="module-desc">short description · interactive</div>
      </div>
    </div>
    <div class="module-right">
      <span class="module-tag">Topic Tag</span>
      <span class="module-arrow">→</span>
    </div>
  </a>
</li>
```

---

*Frank Lato · MS Biomedical Image Computing · UIUC*
