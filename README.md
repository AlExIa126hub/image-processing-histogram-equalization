# Histogram Equalization

Digital Image Processing project exploring histogram equalization for image contrast enhancement.

The project implements both **manual intensity mapping** and **automatic histogram equalization**, allowing comparison of how different equalization strategies affect the appearance and intensity distribution of an image.

---

# Project Structure

```
histogram-equalization/
│
├── notebooks/
│   └── histogram_equalization.ipynb
│
├── data/
│   └── images/
│
└── README.md
```

---

# Project Overview

Histogram equalization is a technique used to improve image contrast by redistributing pixel intensities across the available intensity range.

Images with poor contrast often have intensity values concentrated within a narrow region of the histogram. Histogram equalization spreads these values more evenly, making details more visible.

This project demonstrates how histogram equalization can be implemented both **manually** and **automatically**.

---

# Workflow

The notebook performs the following steps.

---

## 1. Image Loading

The user uploads an image which is used as the input for the processing pipeline.

The original image is displayed along with its corresponding histogram.

---

## 2. Histogram Computation

The histogram of the image is calculated to analyse the distribution of pixel intensities.

The histogram provides insight into:

- brightness distribution
- contrast levels
- potential need for intensity adjustment

---

## 3. Manual Histogram Equalization

The user can manually specify a mapping between input and output intensity values.

This allows direct control over how intensity levels are redistributed and provides insight into how histogram equalization works.

---

## 4. Automatic Histogram Equalization

An algorithm is implemented to perform histogram equalization automatically.

The algorithm:

1. Computes the histogram of the image.
2. Calculates the cumulative distribution function (CDF).
3. Maps original pixel intensities to new values based on the CDF.

This process redistributes intensity values across the full range of available intensities.

---

# Results

The results demonstrate how histogram equalization improves image contrast.

Observations include:

- Dark images become brighter and reveal hidden details.
- Low-contrast images gain a wider intensity distribution.
- The equalized histogram becomes more evenly distributed.

---

# Technologies Used

- Python
- NumPy
- OpenCV
- Matplotlib
- Jupyter Notebook

---

# Running the Project

Clone the repository:

```
git clone <repository-url>
```

Install dependencies:

```
pip install numpy opencv-python matplotlib
```

Launch Jupyter Notebook:

```
jupyter notebook
```

Open and run:

```
notebooks/histogram_equalization.ipynb
```

---

# Concepts Demonstrated

This project demonstrates several key image processing concepts:

- Histogram computation
- Contrast enhancement
- Manual intensity mapping
- Automatic histogram equalization
- Cumulative distribution function (CDF)
