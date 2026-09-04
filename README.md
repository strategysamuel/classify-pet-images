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
