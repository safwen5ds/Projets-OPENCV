# Projet Image - LBP Texture Analysis

**Author:** Gharbi Safwen CI 1

## Description

This project implements Local Binary Pattern (LBP) texture analysis for image processing. It provides an interactive Jupyter notebook interface for uploading images and analyzing their texture characteristics using LBP transformation.

## Features

- **Interactive Image Upload**: User-friendly interface with file upload widget
- **LBP Calculation**: Custom implementation of Local Binary Pattern algorithm
- **Visual Comparison**: Side-by-side display of original and LBP-transformed images
- **Matrix Visualization**: Display of both original and LBP image matrices
- **Histogram Analysis**: Comparative histogram visualization for texture analysis

## Installation

Install the required dependencies:

```bash
pip install opencv-python ipywidgets matplotlib numpy
```

For Google Colab users, the notebook automatically installs the required packages.

## How It Works

### Local Binary Pattern (LBP) Algorithm

The LBP algorithm works by:
1. Converting the image to grayscale
2. For each pixel, comparing its intensity with its 8 neighboring pixels
3. Creating a binary code based on these comparisons
4. Converting the binary code to a decimal value for the new pixel intensity

### Key Functions

- `Calcul_LBP(Img_LBP)`: Implements the LBP transformation algorithm
- `plot_images(org, lbp)`: Displays original and LBP images with their matrices and histograms
- `upload(change)`: Handles file upload and processes the uploaded image
- `display_project()`: Creates the interactive interface

## Usage

1. Run the notebook in Jupyter or Google Colab
2. Use the file upload widget to select an image
3. The system will automatically:
   - Calculate the LBP transformation
   - Display the original and LBP images
   - Show the corresponding matrices
   - Generate histograms for texture analysis

## Output Visualization

The interface displays:
- **Original Image**: The uploaded image in color
- **Original Matrix**: Numerical representation of the grayscale image
- **Original Histogram**: Intensity distribution of the original image
- **LBP Image**: Texture-analyzed version using LBP
- **LBP Matrix**: Numerical representation of the LBP transformation
- **LBP Histogram**: Distribution of LBP values showing texture patterns

## Applications

LBP texture analysis is useful for:
- Texture classification
- Face recognition
- Medical image analysis
- Quality control in manufacturing
- Pattern recognition in various domains

## Technical Details

- **Image Processing**: OpenCV for image manipulation
- **Visualization**: Matplotlib for displaying results
- **Interface**: IPython widgets for interactive experience
- **Environment**: Designed for Google Colab with fallback for local Jupyter

## File Structure

- Main processing code with LBP implementation
- Interactive interface components
- Visualization and display functions 
