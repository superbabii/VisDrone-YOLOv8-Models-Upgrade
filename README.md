# YOLOv8 Models Trained on VisDrone Dataset

This repository contains YOLOv8 models trained on the VisDrone dataset for object detection. It also includes the original YOLOv8 models for reference and comparison.

## Models

The trained models are available in the `visdrone_models` directory. The original YOLOv8 models are available in the `original_models` directory.

## Usage

To use the models, you can download the `.pt` files and load them using the YOLOv8 framework.

### Model Files

Due to GitHub's file size limitations (cannot upload files larger than 100MB), the model files are hosted externally. You can download them from the following links:

- [best(yolov8x-visdrone).pt](https://drive.google.com/file/d/1unATgOABLt1C7RCQ_npGeksXX-jS4vjH/view?usp=sharing)
- [yolov8x.pt](https://drive.google.com/file/d/1uGpYq6hvWmyFP5QuVEixAFHnjO8NBRiU/view?usp=sharing)

These files are too large to upload directly to GitHub.

## Model Performance (Original YOLOv8 Models)

| Model  | Size (pixels) | mAPval 50-95 | Speed CPU ONNX (ms) | Speed A100 TensorRT (ms) | Params (M) | FLOPs (B) |
|--------|---------------|--------------|---------------------|--------------------------|------------|-----------|
| YOLOv8n | 640           | 37.3         | 80.4                | 0.99                     | 3.2        | 8.7       |
| YOLOv8s | 640           | 44.9         | 128.4               | 1.20                     | 11.2       | 28.6      |
| YOLOv8m | 640           | 50.2         | 234.7               | 1.83                     | 25.9       | 78.9      |
| YOLOv8l | 640           | 52.9         | 375.2               | 2.39                     | 43.7       | 165.2     |
| YOLOv8x | 640           | 53.9         | 479.1               | 3.53                     | 68.2       | 257.8     |

## Model Performance (VisDrone-trained YOLOv8 Models)

| Model  | Size (pixels) | Task              | mAPval 50 |
|--------|------------|-------------------|------------|-------------|
| yolov8n-visdrone | 640    | object detection |  34.1     |
| yolov8s-visdrone | 640    | object detection |  40.8     |
| yolov8m-visdrone | 640    | object detection |  45.4     |
| yolov8l-visdrone | 640    | object detection |  46.1     |
| yolov8x-visdrone | 640    | object detection |  47.1     |

### Suitable Uses for YOLOv8 Models

- **YOLOv8n**: Designed for high-speed applications with low computational resources, making it suitable for edge devices.
- **YOLOv8s**: Ideal for real-time applications requiring moderate computational power, such as real-time video processing.
- **YOLOv8m**: A balanced model offering good performance and speed, suitable for general object detection tasks.
- **YOLOv8l**: Provides high accuracy, making it suitable for detailed image analysis and complex environments.
- **YOLOv8x**: The most accurate model, best suited for applications where the highest accuracy is critical, such as research and development in AI and computer vision.

## Resources

- VisDrone Dataset: [VisDrone-Dataset on GitHub](https://github.com/VisDrone/VisDrone-Dataset)
- YOLOv8: [Ultralytics YOLOv8 on GitHub](https://github.com/ultralytics/ultralytics)
- YOLOv8 Training Documentation: [YOLOv8 Training Documentation](https://docs.ultralytics.com/modes/train/#key-features-of-train-mode)
- Using VisDrone with YOLOv8: [VisDrone Usage Documentation](https://docs.ultralytics.com/datasets/detect/visdrone/#usage)

## Training

The training scripts and configuration files are available in the `scripts` directory. For more details on how to train YOLOv8 models, refer to the YOLOv8 training documentation.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
