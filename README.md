# Object Detection Project

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Torch](https://img.shields.io/badge/Torch-1.7%2B-red)
![supervision](https://img.shields.io/badge/supervision-0.1%2B-green)
![OpenCV](https://img.shields.io/badge/OpenCV-4.5%2B-red)
![NumPy](https://img.shields.io/badge/NumPy-1.19%2B-orange)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.3%2B-yellow)
![Pandas](https://img.shields.io/badge/Pandas-1.1%2B-green)

This project focuses on object detection using the Grounding DINO model, leveraging the COCO dataset for training and evaluation. The implementation utilizes various libraries such as PyTorch, Supervision, and others to perform detection tasks and manage datasets in COCO format.

## Libraries and Tools

- **PyTorch**: Utilized for model loading, prediction, and annotation.
- **Grounding DINO**: A specialized object detection model used for this project.
- **Supervision**: For data handling and visualization.
- **Google Colab**: For integrating with Google Drive and managing datasets.

## Project Overview

The primary goal of this project is to detect and annotate objects within images, utilizing a pre-trained Grounding DINO model. The model is fine-tuned and evaluated using images from the COCO dataset, a widely used dataset in the object detection field.

### Key Features

- **Model Loading and Prediction**: The project includes code to load the Grounding DINO model and perform predictions on input images.
- **Dataset Management**: Images are loaded from Google Drive, with annotations formatted according to the COCO dataset specifications.
- **Visualization**: Detected objects are visualized with bounding boxes and labels.

### COCO Dataset Format

The project outputs annotations in the COCO dataset format, which is essential for maintaining consistency and compatibility with other tools and models in the object detection ecosystem. Annotations are generated for each individual image as well as combined into a single file for all images.

#### Example COCO Annotation

```json
{
  "images": [
    {
      "id": 34,
      "coco_url": "https://images.cocodataset.org/val2014/000000000034.jpg"
    }
  ],
  "annotations": [
    {
      "image_id": 34,
      "bbox": [x, y, width, height],
      "category_id": 1,
      "score": 0.9
    }
  ],
  "categories": [
    {
      "id": 1,
      "name": "object"
    }
  ]
}
```

## Example: Detection and Annotation

Below is an example of how the model detects and annotates objects in an image:

### Input Image

![000000000034](https://github.com/user-attachments/assets/e90be6dc-b39e-4845-8409-8c0faaa8a761)


### Output Annotation

The model detects parts of the body, such as eyes and ears, with the following annotation:
- **Bounding Box**: `[x, y, width, height]`
- **Category**: `part of body`
- **Confidence Score**: `0.9`

### Visualization

![image](https://github.com/user-attachments/assets/1dc4de1f-2bba-4a1d-9c1d-f187e0b3d0aa)


## Conclusion

This project demonstrates a comprehensive approach to object detection using advanced models and well-structured datasets. By leveraging the power of PyTorch and Grounding DINO, it achieves accurate and efficient object detection, with results formatted in the widely recognized COCO dataset format.

## More expamples 

| Objects to find | Input Image | Visualization |
| ------- | ------- | -------- |
| Text, plane | ![000000000081](https://github.com/user-attachments/assets/91e162d2-3e2c-4c58-bd3d-8e644480b0f7) | ![image](https://github.com/user-attachments/assets/a0f8abdb-3be1-4c29-be60-be23e7a3bbfb) |
| Knifes, Stove | ![000000000089](https://github.com/user-attachments/assets/3de0c729-7c69-417b-abc3-6dbb11a06248) | ![image](https://github.com/user-attachments/assets/46178ff4-726d-449d-acbd-cb3016ccdc03) |
| People | ![000000000109](https://github.com/user-attachments/assets/549a90db-df3d-409e-b2df-2013318ddd6a) | ![image](https://github.com/user-attachments/assets/1decd93f-625e-42d8-84a4-af910f75a5b5) |





