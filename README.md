# Implementation of Opening and Closing

## Aim

To implement Opening and Closing morphological operations using Python and OpenCV.

---

## Objective

The objective of this experiment is to perform Opening and Closing operations on a noisy image using OpenCV in order to remove noise and improve image quality.

---

## Software Required

- Python 3.x
- OpenCV (`cv2`)
- NumPy
- Matplotlib
- Jupyter Notebook / VS Code

---

## Theory

Morphological operations are image processing techniques used to process images based on shapes and structures.

### Opening
Opening is performed by applying erosion followed by dilation. It helps remove small white noise from the image while preserving the overall shape of the object.

### Closing
Closing is performed by applying dilation followed by erosion. It helps fill small holes and gaps inside the foreground object.

These operations are widely used in noise removal and image preprocessing applications.

---

## Algorithm

### Step 1:
Import the required libraries such as OpenCV, NumPy, and Matplotlib.

### Step 2:
Create a blank image and generate text using the `cv2.putText()` function.

### Step 3:
Generate white noise using `np.random.randint()`.

### Step 4:
Add the generated noise to the image.

### Step 5:
Create a structuring element (kernel) using NumPy.

### Step 6:
Apply Opening operation using `cv2.morphologyEx()` with `cv2.MORPH_OPEN`.

### Step 7:
Apply Closing operation using `cv2.morphologyEx()` with `cv2.MORPH_CLOSE`.

### Step 8:
Display the noisy image, opening result, and closing result.

---

## OpenCV Functions Used

| Function | Purpose |
|---|---|
| `cv2.putText()` | Create text image |
| `np.random.randint()` | Generate white noise |
| `cv2.morphologyEx()` | Perform opening and closing |
| `np.ones()` | Create kernel |
| `plt.imshow()` | Display image |

---

## Expected Output

The program produces the following outputs:

- Original text image
- Noisy image
- Opening output image
- Closing output image

---

## Applications

- Noise removal
- Image preprocessing
- Medical image processing
- Character recognition
- Shape enhancement
- Object segmentation

---

## Result

Thus, the Opening and Closing morphological operations are successfully implemented using Python and OpenCV. The noise present in the image is reduced and image quality is improved.

---

## Developed By

**Name:** THIRUMALAI K

**Register Number:** 212224240176