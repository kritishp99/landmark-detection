# Landmark Detection Using Deep Learning

## Project Overview

This project explores image-based landmark classification using Deep Learning and the VGG19 convolutional neural network architecture.

The objective is to process landmark images and classify them according to their corresponding landmark IDs.

The project uses Python, Keras, OpenCV, and image-processing techniques to prepare the dataset and build a deep learning model.

## Technologies Used

- Python
- TensorFlow / Keras
- VGG19
- OpenCV
- NumPy
- Pandas
- Matplotlib
- Pillow (PIL)

## Dataset

The notebook uses a landmark image dataset containing image IDs and their corresponding landmark IDs.

The dataset is loaded using a CSV file named `train.csv`.

The image files are stored in an `images` directory.

**Dataset columns:**
- `id` – Unique image identifier.
- `landmark_id` – Corresponding landmark class identifier.

The notebook identifies 5,346 distinct landmark classes in the displayed dataset summary.

**Note:** The dataset files are not included in this repository. You must provide the CSV file and image directory separately to run the notebook.

## Model Architecture

The project uses the VGG19 convolutional neural network architecture for image-based feature extraction and classification.

### Model Configuration

| Parameter | Value |
|---|---|
| Architecture | VGG19 |
| Input Image Size | 224 × 224 |
| Batch Size | 16 |
| Epochs Configured | 1 |
| Pretrained Weights | None |

## Project Structure

```text
landmark-classification/
│
├── Landmark_Detection.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/kritishp99/landmark-classification.git
```

### 2. Navigate to the project directory

```bash
cd landmark-classification
```

### 3. Install the required libraries

```bash
pip install -r requirements.txt
```

### 4. Prepare the dataset

Place the dataset files in the following structure:

```text
landmark-classification/
│
├── train.csv
├── images/
│   ├── image1.jpg
│   ├── image2.jpg
│   └── ...
```

The image filenames and CSV identifiers must match the format expected by the notebook.

### 5. Run the notebook

Open `Landmark_Detection.ipynb` using Jupyter Notebook or Google Colab and execute the cells in order.

## Current Implementation

The notebook includes:

- Loading landmark image metadata from CSV.
- Exploring landmark IDs and image records.
- Image processing using OpenCV and PIL.
- Preparing image data for deep learning.
- Configuring a VGG19-based neural network.

**Note:** The current notebook does not yet contain a completed model training and evaluation workflow. Accuracy and prediction results will be added after training and testing are implemented.

## Future Improvements

- Complete model training and validation.
- Evaluate the model using accuracy and loss metrics.
- Experiment with pretrained VGG19 weights.
- Improve image preprocessing and data augmentation.
- Add landmark prediction for new images.
- Develop a simple interface for image-based landmark recognition.

## Conclusion

This project explores the use of Convolutional Neural Networks for landmark image classification. It provides a foundation for building a deep learning system that can recognize landmarks from images.

---

**Project:** Landmark Detection  
**Domain:** Deep Learning / Computer Vision  
**Architecture:** VGG19  
**Language:** Python

**GitHub:** https://github.com/kritishp99/landmark-classification
