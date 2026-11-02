# Medical Image Preprocessing and Analysis Using Python

## Project Overview

### This project explores basic image preprocessing techniques using Python and medical MRI images. The main goal is to understand how different preprocessing methods affect image quality and visual details.

## Dataset

### A small sample of brain MRI images was selected from the Brain Tumor Detection dataset.
**Dataset Source:** [Brain Tumor Detection Dataset](https://github.com/ahmedhamada0/Brain-Tumor-Detection)
	 Images were selected from the Training folder.
     5 Healthy images and 5 Tumor images were used.

## Preprocessing Methods

### The following techniques were applied: 

   1. **Grayscale Conversion:** Converted RGB images into grayscale.
   2. **Image Resizing:** Resized all images to 256 × 256 pixels.
   3. **Gaussian Blur:** Applied Gaussian filtering with radius = 2.
   4. **Median Filter:** Applied median filtering with a 3 × 3 window.
   5. **Contrast Enhancement:** Increased image contrast using a factor of 1.5.

## Tools and Libraries
	•	Python
	•	NumPy
	•	Matplotlib
	•	Pillow (PIL)
	•	Pandas
    •   os module
	•	Jupyter Notebook

## Results and Observations

### The selected images were visually compared after applying different preprocessing techniques.
	•	Gaussian Blur produced smoother images but also blurred some visible details.
	•	Median Filter preserved more visible details than Gaussian Blur in the selected sample images.
	•	Contrast Enhancement improved the visual distinction between some bright and dark regions.
	•	Grayscale conversion and resizing provided standardized images for further processing.

## Limitations
	•	The initial analysis was performed on small sample of MRI images.
	•	Results were evaluated through visual comparison.
	•	No deep learning model or medical diagnostic system was developed.
	•	The observations should not be generalized to the entire dataset.

## Project Structure

```text
Medical_Image_Processing/
│
├── images/
│   ├── healthy/
│   └── tumor/
│
├── results/
│   ├── grayscale_resized/
│   ├── gaussian/
│   ├── median/
│   └── contrast/
│
├── Medical_Image_Processing.ipynb
└── README.md
```

## How to Run

1. Install Python.
2. Install the required libraries:
```bash
pip install numpy matplotlib pillow pandas
```
3. Open Jupyter Notebook.
4. Run the notebook cells in order.

## Future Improvements

- Evaluate preprocessing techniques using larger image samples.
- Explore quantitative image quality metrics where suitable reference images are available.
- Investigate additional image enhancement techniques.
- Explore deep learning methods for medical image analysis in future work.
