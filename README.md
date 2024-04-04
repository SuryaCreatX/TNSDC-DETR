# DETR Image Inference Model

This project implements an image inference model based on Facebook's DETR (DEtection TRansformer) architecture. The DETR model is a transformer-based neural network designed for object detection tasks. Unlike traditional methods that rely on anchor boxes, DETR directly predicts object bounding boxes and class labels in a single pass.

![DETR Infrencing](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*ooeDTYZhMTAcHSgDAqHeuw.png)

## How it Works

1. **Initialization**: The project begins by initializing the necessary components. It loads the pre-trained DETR model and the feature extractor.
2. **Image Encoding**: The input image is passed through the feature extractor to obtain its encoded representation. This encoding captures important features of the image.
3. **Inference**: The encoded image is then fed into the DETR model for inference. The model predicts the bounding boxes and class labels for objects detected in the image.
4. **Post-processing**: After obtaining the model predictions, post-processing is performed to refine the bounding boxes and filter out low-confidence detections. The bounding boxes are scaled appropriately to match the dimensions of the input image.
5. **Visualization**: Finally, the results of the object detection are visualized by drawing bounding boxes around the detected objects and labeling them with their corresponding class labels.

## Features

- **Efficient Object Detection**: Utilizes the DETR architecture for efficient object detection.
- **Pre-trained Weights**: Pre-trained weights on the COCO dataset for quick deployment.
- **Simple Interface**: Provides a straightforward interface for running inference on images.
- **Visualization**: Capable of visualizing detection results with bounding boxes and class labels.

## Usage

1. **Clone the Repository**:

    ```
    git clone https://github.com/your_username/detr_image_inference.git
    cd detr_image_inference
    ```

2. **Run Inference**
   To run the inference, provide the URL of the image to be analyzed. For example:

   ```
   'http://farm8.staticflickr.com/7351/9196825828_4200f7681e_z.jpg'
   ```
   From the COCO dataset.

## Example Results

![Example Result](https://miro.medium.com/v2/resize:fit:828/format:webp/1*zUc-SPbJNM_MD5m3c5ADPQ.jpeg)

Above is an example result of object detection using the DETR model on an input image.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
   
