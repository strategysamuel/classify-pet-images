# Classify Pet Images

## Project Overview

This project is part of the Udacity AI Programming with Python Nanodegree.

The objective is to use a pretrained Convolutional Neural Network (CNN) image classifier to:

1. Identify which pet images are dogs and which are not dogs.
2. Classify the breed of dogs in the images.
3. Compare the performance of three pretrained CNN architectures:
   - ResNet
   - AlexNet
   - VGG

The project uses the supplied `classifier.py` module and does not train a CNN from scratch.

## Project Structure

| File / Folder | Description |
|---|---|
| `check_images.py` | Main program that runs the image classification workflow |
| `get_input_args.py` | Processes command-line arguments |
| `get_pet_labels.py` | Extracts pet labels from image filenames |
| `classify_images.py` | Classifies images using a pretrained CNN |
| `adjust_results4_isadog.py` | Determines dog/not-dog classifications |
| `calculates_results_stats.py` | Calculates classification statistics |
| `print_results.py` | Prints the final results |
| `classifier.py` | Supplied pretrained CNN classifier |
| `dognames.txt` | List of recognized dog breeds |
| `pet_images/` | Pet image dataset |
| `uploaded_images/` | Additional test images |
| `run_models_batch.sh` | Script for running multiple CNN architectures |

## How to Run

Run the program from the project directory:

```bash
python check_images.py

The default configuration uses:

- Directory: `pet_images/`
- Architecture: `vgg`
- Dog names file: `dognames.txt`

A specific architecture can be selected using:

```bash
python check_images.py --dir pet_images/ --arch resnet --dogfile dognames.txt

python check_images.py --dir pet_images/ --arch alexnet --dogfile dognames.txt

python check_images.py --dir pet_images/ --arch vgg --dogfile dognames.txt

Results

The project dataset contains 40 pet images:

30 dog images
10 non-dog images
VGG
Metric	Result
Dog Classification Accuracy	100.0%
Non-Dog Classification Accuracy	100.0%
Dog Breed Classification Accuracy	93.3%
Pet Label Match	87.5%

VGG produced the best dog breed classification performance.

ResNet
Metric	Result
Dog Classification Accuracy	100.0%
Non-Dog Classification Accuracy	90.0%
Dog Breed Classification Accuracy	90.0%
AlexNet
Metric	Result
Dog Classification Accuracy	100.0%
Non-Dog Classification Accuracy	100.0%
Dog Breed Classification Accuracy	80.0%
VGG Misclassified Dog Breeds

The VGG model correctly identified all dog images as dogs. Two breed classifications did not match the labels derived from the image filenames:

Great Pyrenees → Kuvasz
Beagle → Walker Hound / Walker Foxhound
Key Learning Outcomes

This project demonstrates:

Python command-line argument processing
Working with dictionaries and files
Image classification using pretrained CNN architectures
Comparing model performance
Calculating classification accuracy
Identifying dogs versus non-dogs
Evaluating dog breed classification
Measuring program execution time
Using Git and GitHub for version control
Technologies Used
Python
PyTorch
Torchvision
Pretrained CNN architectures
Git
GitHub
Author

A Samuel Arun Kumar
