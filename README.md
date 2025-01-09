# OCR National ID and Bank Card Classifier

This project focuses on Optical Character Recognition (OCR) for identifying whether an image is a **National ID card** or a **Bank Card**. The classifier processes images to extract important features and identifies the card type through image processing techniques and template matching. The project also incorporates components to detect and classify various elements, such as card numbers, expiration dates, and more.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Project Overview](#project-overview)
- [Results](#results)
- [Contributors](#contributors)
<!-- - [License](#license) -->

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/mspoulaei/ocr-card-classifier.git
    cd ocr-card-classifier
    ```

2. Install required dependencies like cv2 and keras

3. Ensure you have Jupyter Notebook installed to run the project.

## Usage

To run the classifier, open the Jupyter Notebook `checker.ipynb`:

1. Launch Jupyter Notebook:

    ```bash
    jupyter notebook
    ```

2. Open `checker.ipynb` and run the cells step by step.

The notebook will guide you through:

- Reading and pre-processing the image.
- Determining whether the image is a National ID or Bank Card.
- Applying morphological transformations and adaptive thresholding.
- Identifying key features (numbers, dates) using template matching or deep learning techniques.
- Displaying the results.

## Project Overview

### Problem

The goal of the project is to develop a system that can:

- Differentiate between a **National ID card** and a **Bank Card** from an image.
- Detect numbers and text present on the card.
  
The image processing steps include:

- **Image Preprocessing**: Conversion to grayscale, denoising, and sharpening.
- **Morphological Operations**: `opening`, `closing`, `dilate`, and `erode` to enhance key features.
- **Contour Detection**: Extracting and analyzing contours to locate card boundaries.
- **Template Matching**: Identifying specific templates, such as card numbers or dates, within the image.

### Techniques Used

- **Adaptive Thresholding**: To convert images to binary for easier feature extraction.
- **Morphological Transformations**: Used to clean up the image and reduce noise.
- **Template Matching**: To locate and classify numbers, card details, etc.
- **Deep Learning**: A deep learning model based on the MNIST dataset was used to further improve number classification.

## Results

The project successfully identifies whether the input image is a **National ID** or **Bank Card**. It accurately detects numbers and key features such as:

- National ID number
- Expiration date
- CVV/CVV2

The results are displayed by drawing bounding boxes around detected numbers or card elements.

<!-- Sample output: -->

<!-- ![Sample Output](path-to-output-image) -->

## Contributors

- **Mohammad Sadegh Poulai Mozirji**
- **Sayin Ala**

Supervised by:

- **Dr. Mohammadi**

<!-- ## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. -->
