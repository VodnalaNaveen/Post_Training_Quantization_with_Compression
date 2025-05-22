# Model Compression Using TensorFlow Lite (Without Quantization)

This project demonstrates how to compress a trained Keras model by converting it to the TensorFlow Lite (TFLite) format. This form of compression reduces the model size, making it more lightweight and faster to load — suitable for environments with limited storage or memory, such as mobile or embedded devices. However, no numerical approximation (like quantization) is applied — model weights remain in float32 precision.

## What Can a Quantized Model (Compression) Do for Me?
  * Reduce model size significantly while maintaining full-precision accuracy (float32)
  * Speeds up model loading
  * Lower memory and power usage

## Getting Started
### 1. Create an Environment
``` conda create -n compressed_model python==3.12 ```
### 2.Activate the Environment
``` conda activate compressed_model ```
### 3.Install Project Dependencies
``` pip install -r requirements.txt ```
## Run the code
```
python .\run.py --weights_path "C:\Users\vodna\OneDrive\Desktop\QUANTIZATION\Elite28_PQT\normal.h5" --num_preds 5 --compressed_model_path 'C:\Users\vodna\OneDrive\Desktop\compresed_model'
```
#### Parser Arguments

 * --weights_path	         :-	Path of your original .h5 model
 * --compressed_model_path	:-	Folder path to save compressed model
