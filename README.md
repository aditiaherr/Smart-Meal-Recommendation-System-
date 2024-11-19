# Smart Meal Recommendation System

This project presents a Smart Meal Recommendation System that utilizes advanced computer vision techniques to streamline the meal preparation process. By employing the YOLO (You Only Look Once) object detection algorithm, the system is capable of detecting various food ingredients from images captured in real-time. Once the ingredients are identified, they are cross-referenced with a comprehensive database of recipes to suggest appropriate meal options tailored to the user's available ingredients.

The goal is to make meal planning easier, reduce food wastage, and encourage creativity in cooking by suggesting meal ideas based on the ingredients you already have.

## Abstract

This project aims to develop a Smart Meal Recommendation System using computer vision techniques and the YOLO object detection algorithm to identify food ingredients. By utilizing YOLO, the system can recognize 94 distinct ingredients and suggest recipes based on those ingredients. The system is designed to automate meal planning by allowing users to take a snapshot of the ingredients they have and receive tailored recipe suggestions. The project integrates a recipe database and provides an intuitive user interface for quick interaction, enhancing the cooking experience and reducing food waste.

The dataset consists of 94 food ingredients, annotated and labeled using the Roboflow platform for high accuracy in ingredient detection. The system empowers users to make the best use of available resources and discover new recipes with ease.

## Table of Contents

1. [Introduction](#introduction)
2. [Project Design](#project-design)
3. [Module Description](#module-description)
4. [Results](#results)
5. [Conclusion](#conclusion)
6. [References](#references)
7. [Plagiarism Report](#plagiarism-report)

## Screenshots

Here are some screenshots from the project:

- ![Result 4](https://github.com/aditiaherr/Smart-Meal-Recommendation-System-/blob/main/result_4.jpeg)
- ![Result 6](https://github.com/aditiaherr/Smart-Meal-Recommendation-System-/blob/main/result_6.jpeg)

## Chapter 1: Introduction

### Problem Statement

In modern fast-paced lifestyles, many individuals struggle with meal planning due to time constraints and a lack of culinary inspiration. Often, people resort to takeout or repetitive meals, leading to food wastage and unhealthy eating habits. This project aims to tackle this problem by leveraging YOLO-based object detection to automatically recognize ingredients and suggest recipes based on them.

### Project Idea

This project integrates computer vision technology with a user-friendly interface to suggest meals based on available ingredients. By taking a snapshot of the ingredients, the system suggests relevant recipes, promoting better food utilization and creativity in cooking.

### Motivation

The motivation behind this project is to reduce food waste, promote healthy eating, and inspire creativity in cooking. This system encourages users to explore different meal options based on what they have, without the need for detailed planning.

### Scope

- Detect 94 different food ingredients using YOLO.
- Integrate a recipe database.
- Provide recipe recommendations based on detected ingredients.

### Literature Survey / Requirement Analysis

A review of related works highlights the need for an object detection-based meal recommendation system. Existing solutions either rely on manual input of ingredients or lack real-time detection. This system aims to improve both aspects by automating ingredient detection.

## Chapter 2: Project Design

### Hardware & Software Requirements

#### Hardware:
- Computer with at least 8 GB RAM and a dedicated GPU for model training and inference.
- Webcam or camera-enabled device for capturing images.

#### Software:
- Python for development.
- YOLO for object detection.
- OpenCV for image processing.
- Roboflow for dataset creation and annotation.
- Recipe database stored in CSV format.

### Dataset Design

The dataset consists of 94 different food ingredients, each annotated using Roboflow. The ingredients are captured under various lighting conditions and orientations to improve the accuracy of detection.

### Hours Estimation

- Dataset Creation and Annotation: 20 hours
- Model Training and Tuning: 30 hours
- Recipe Database Development: 15 hours
- User Interface Design: 25 hours
- Testing and Documentation: 10 hours

**Total Estimated Hours**: 100 hours

## Chapter 3: Module Description

### Block Diagram

![Block Diagram](images/block_diagram.png)

1. **User Interface**: Allows users to capture images and interact with the system.
2. **Image Capture**: Captures real-time images of ingredients.
3. **YOLO Object Detection Model**: Identifies food ingredients in the captured image.
4. **Ingredient List**: Displays the detected ingredients.
5. **Recipe Database**: A collection of recipes linked to ingredients.
6. **Recipe Suggestion**: Provides recipe recommendations based on the detected ingredients.

### System Architecture

![System Architecture](images/system_architecture.png)

The YOLOv5 architecture is used for real-time object detection. YOLOv5 is highly efficient, fast, and capable of detecting objects with high accuracy. The system leverages YOLOv5’s feature extraction capabilities using CSPDarknet53 and PANet to achieve better detection results.

## Chapter 4: Results

### Screenshots

- ![Result 4](https://github.com/aditiaherr/Smart-Meal-Recommendation-System-/blob/main/result_4.jpeg)
- ![Result 6](https://github.com/aditiaherr/Smart-Meal-Recommendation-System-/blob/main/result_6.jpeg)

### Test Cases

Test cases were executed to ensure that the system provides accurate recommendations based on the ingredients detected in the images. The precision and recall curves for the model are shown below:

- ![Recall-Confidence Curve](images/recall_curve.png)
- ![Precision-Confidence Curve](images/precision_curve.png)
- ![Precision-Recall Curve](images/precision_recall_curve.png)

## Chapter 5: Conclusion

This project successfully demonstrates the use of YOLO for real-time food ingredient detection and recipe suggestion. It provides a practical solution for meal planning and reduces food waste by encouraging users to cook based on the ingredients they already have. Future work can include adding nutritional information and supporting dietary preferences.


