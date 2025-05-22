# Post Training Quantization Model Compression

This project demonstrates how to compress a trained Keras model using post-training quantization with TensorFlow Lite, reducing model size and enabling faster, resource-efficient inference—ideal for deployment on mobile and embedded systems.

# What Can a Quantized Model (Compression) Do for Me?
  * Reduce model size significantly without retraining
  * Speed up inference on edge devices
  * Lower memory and power usage

# Getting Started
### 1. Create an Environment
``` conda create -n compressed_model python==3.12 ```
### 2.Activate the Environment
``` conda activate compressed_model ```
### 3.Install Project Dependencies
``` pip install -r requirements.txt ```
# Run the code
```
python .\run.py --weights_path "C:\Users\vodna\OneDrive\Desktop\QUANTIZATION\Elite28_PQT\normal.h5" --num_preds 5 --compressed_model_path 'C:\Users\vodna\OneDrive\Desktop\compresed_model'
```
#### Parser Arguments

 * --weights_path	         :-	Path of your original .h5 model
 * --data_path	            :-	Path to input CSV file (default: ./data.csv)
 * --num_preds	            :-	Number of predictions to make
 * --compressed_model_path	:-	Folder path to save compressed model
