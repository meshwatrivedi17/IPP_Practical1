[README_Practical-1.md](https://github.com/user-attachments/files/34223100/README_Practical-1.md)
# Image Processing & Pattern Recognition – Practical 1

**Topic:** Image basics and fundamental operations
**Notebook:** `IPP_Practical-1.ipynb`
**Course:** PGDM in Big Data Analytics (AI & DS), AIDTM (Batch 2025–27)

---

##  Overview

This practical covers the fundamentals of working with images in Python: reading, displaying, converting, transforming and comparing them using **OpenCV**, **Pillow**, **Matplotlib** and **scikit-image**.

---

##  Tech Stack

| Library | Purpose |
|---|---|
| OpenCV (`cv2`) | Image I/O, colour conversion, resize, rotate, flip |
| Pillow (PIL) | Image loading |
| NumPy | Array and pixel operations |
| Matplotlib | Displaying images |
| scikit-image | Mean Squared Error calculation |

---

##  Tasks Covered

| # | Task | Technique |
|---|---|---|
| 1 | Read `flower.jpg` and display it as "Original Image" | `cv2.imread`, BGR → RGB, `plt.imshow` |
| 2 | Print dimensions and data type of `scene.jpg` | `img.shape`, `img.dtype` |
| 3 | Convert a colour image to grayscale and save as `output_gray.jpg` | `cv2.cvtColor`, `cv2.imwrite` |
| 4 | Open `sunset.png` using Pillow and display it | `Image.open` |
| 5 | Resize an image to 50% of its width and height | `cv2.resize` |
| 6 | Crop the central 200×200 pixel area | NumPy array slicing |
| 7 | Rotate an image 90° clockwise | `cv2.rotate` |
| 8 | Flip `car.jpg` left-to-right | `cv2.flip(img, 1)` |
| 9 | Convert to HSV and display Hue, Saturation and Value separately | `cv2.split`, Matplotlib subplots |
| 10 | Compute MSE between two grayscale images | `mean_squared_error` |

---

##  Results

- **Image shape of `scene.jpg`:** `(455, 674, 3)` (height, width, channels)
- **Data type:** `uint8`
- **MSE between `img1.jpg` and `img2.jpg`:** ≈ `8450.40`

---

##  Input Images Required

Place these files in the same folder as the notebook:

`flower.jpg`, `scene.jpg`, `sunset.png`, `car.jpg`, `img1.jpg`, `img2.jpg`

---

##  How to Run

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>

# 2. Install dependencies
pip install opencv-python pillow numpy matplotlib scikit-image jupyter

# 3. Launch Jupyter and open the notebook
jupyter notebook IPP_Practical-1.ipynb
```

---

##  Key Learnings

- OpenCV loads images in **BGR** order, so they must be converted to RGB before displaying with Matplotlib.
- Image properties such as shape and dtype describe how the pixel data is stored.
- Geometric operations (resize, crop, rotate, flip) can be done with a single OpenCV or NumPy call.
- HSV separates colour (Hue) from intensity (Value), which is useful for colour-based analysis.
- MSE gives a numerical measure of how different two images are.

---

##  Author

**Meshwa**
PGDM – Big Data Analytics, AIDTM
