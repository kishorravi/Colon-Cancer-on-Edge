# AI Image Classification on STM32 using MobileNetV3

## Overview

This project demonstrates how to deploy a deep learning model on an STM32 microcontroller for real-time image classification. The model was trained using PyTorch, exported to the ONNX format, and deployed to the STM32 platform using ST Edge AI Suite.

## Features

* MobileNetV3-Small deep learning model
* Trained using PyTorch
* Exported to ONNX format
* Optimized with ST Edge AI Suite
* Real-time AI inference on STM32
* Embedded AI deployment

## Project Workflow

1. Train the MobileNetV3-Small model in PyTorch.
2. Export the trained model to ONNX.
3. Import the ONNX model into ST Edge AI Suite.
4. Optimize and generate embedded C code.
5. Import the generated files into STM32CubeIDE.
6. Build and flash the firmware to the STM32 development board.
7. Run real-time inference on the STM32 device.

## Project Structure

```text
├── model/
│   ├── best_mobilenetv3_small.pth
│   ├── best_mobilenetv3_small.onnx
│   └── best_mobilenetv3_small.onnx.data
│
├── stm32_project/
│   ├── Core/
│   ├── Drivers/
│   ├── AI/
│   └── STM32CubeIDE Project Files
│
├── images/
├── README.md
```

## Technologies Used

* STM32 Microcontroller
* STM32CubeIDE
* ST Edge AI Suite
* PyTorch
* ONNX
* Python
* MobileNetV3-Small

## Model Deployment

The trained PyTorch model (`.pth`) was exported to the ONNX format. ST Edge AI Suite converts the ONNX model into optimized embedded C code that runs efficiently on STM32 microcontrollers.

## Files

| File                               | Description                          |
| ---------------------------------- | ------------------------------------ |
| `best_mobilenetv3_small.pth`       | Trained PyTorch model                |
| `best_mobilenetv3_small.onnx`      | ONNX model used for deployment       |
| `best_mobilenetv3_small.onnx.data` | External model weights (if required) |

## Requirements

* STM32CubeIDE
* ST Edge AI Suite
* Python 3.x
* PyTorch
* ONNX
* STM32 Development Board

## Results

The deployed model performs image classification directly on the STM32 microcontroller without requiring cloud processing, enabling low-latency and energy-efficient AI inference on embedded hardware.

## Future Improvements

* INT8 quantization
* Real-time camera input
* Performance benchmarking
* Support for additional CNN models
* Edge AI optimization

## Author

Kishor Ravikumar

GitHub: https://github.com/your-github-username
