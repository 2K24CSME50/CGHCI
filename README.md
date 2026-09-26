# CGHCI
# Week 02 Lab – Image Processing

This repository contains the complete solutions for the Week 02 Image Processing Lab using Python and NumPy. Each problem includes the required explanation, mathematical rule, manual calculation, Python implementation, testing, and output.

## Problems Covered

### Problem 1 – Image Thresholding

Converts a grayscale image into a binary image using a threshold value.

**Rule:**

```text
If pixel >= threshold → 255
If pixel < threshold  → 0

Example:

Input:
20   128   200
100  150   250

Threshold = 128

Output:
0   255   255
0   255   255

File: Problem1_Thresholding.ipynb

Problem 2 – Image Memory
Calculates the memory required to store an image based on its width, height, and bits per pixel.

Formula:
Memory (bytes) = Width × Height × Bits Per Pixel / 8

Example:
Width  = 1920
Height = 1080
BPP    = 24

Memory = 1920 × 1080 × 24 / 8
       = 6,220,800 bytes

File: Problem2_Image_Memory.ipynb

Problem 3 – Average 9 Pixels
Calculates the rounded average of nine pixels in a 3 × 3 image block.

Formula:
Average = Sum of all 9 pixels / 9
Example:
10   20   10
30   50   30
10   20   10

Sum = 190
Average = 190 / 9
        = 21.11
Rounded Average = 21

File: Problem3_Mean_Filter.ipynb
Problem 4 – Change Image Contrast

Changes image values from one range to another using contrast stretching.

Formula:
new_value =
(value - old_min) / (old_max - old_min)
× (new_max - new_min) + new_min

Example:
Input:
[50, 100, 150]

Old Range:
[50, 150]

New Range:
[0, 255]

Output:
[0, 127.5, 255]

File: Problem4_Contrast.ipynb

Problem 5 – Sobel Edge Detection
Uses Sobel filters to calculate the horizontal edge response, vertical edge response, and overall edge strength of a 3 × 3 grayscale image block.
Gx Kernel:
-1   0   1
-2   0   2
-1   0   1
Gy Kernel:
-1  -2  -1
 0   0   0
 1   2   1
Edge Strength:
Edge Strength = √(Gx² + Gy²)
Example Result:
Gx = 720
Gy = 0
Edge Strength = 720

File: Problem5_Sobel.ipynb

Lab Structure

Each problem follows four main steps:
Inputs and Outputs
Mathematical Rule
Manual Trace
Python Implementation

Each notebook also includes testing to verify the correctness of the solution.

Technologies Used
Python
NumPy
Jupyter Notebook
VS Code
Git
GitHub

Repository Structure

Week02-Lab/
│
├── Problem1_Thresholding.ipynb
├── Problem2_Image_Memory.ipynb
├── Problem3_Mean_Filter.ipynb
├── Problem4_Contrast.ipynb
├── Problem5_Sobel.ipynb
└── README.md

How to Run
Install Python.
Install NumPy:

pip install numpy

Open the repository in VS Code.
Open any .ipynb file.
Select the Python kernel.
Run the notebook cells.

Learning Objectives

This lab provides practical experience with:
Image thresholding
Binary image conversion
Image memory calculation
Bits and bytes
Mean filtering
Pixel averaging
Contrast stretching
Image value transformation
Sobel edge detection
NumPy arrays
Python functions
Mathematical calculations
Testing and verification

Testing

Each problem contains a test section. A successful test displays:

Problem X passed

This confirms that the implementation produces the expected result for the given test case.

Author
Name: Zeeshan Ahmed
Course: Computer Science
Lab: Week 02 – Image Processing

Conclusion
This repository demonstrates the implementation of five fundamental image processing problems using Python and NumPy. The solutions combine mathematical concepts with practical programming and include explanations, manual calculations, implementations, tests, and outputs.
