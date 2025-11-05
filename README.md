Vision-Aided Intelligence with Visual Question Answering (VQA) for Medical Imaging
 Overview

This project introduces an AI-powered Visual Question Answering (VQA) model designed for medical imaging, specifically focused on detecting and grading Diabetic Macular Edema (DME) using fundus images.
By combining VGG16, Word2Vec, and LSTM, the model interprets both images and text-based questions to deliver accurate, explainable, and consistent medical insights — achieving a training accuracy of 96.88% and validation accuracy of 87.52%.

Objectives

1.Develop a multimodal VQA system integrating visual and textual data for medical applications.

2.Improve diagnostic accuracy and logical consistency in AI-generated medical answers.

3.Enhance trust, interpretability, and efficiency in clinical decision support systems.

4.Benchmark against traditional models like ResNet101, showing superior performance in DME grading.

Key Features

1. Visual Feature Extraction – Uses VGG16 to capture fine retinal image details.
2. Text Understanding – Employs Word2Vec and LSTM for semantic understanding of medical questions.
3. Multimodal Fusion – Combines image and text embeddings for contextual question answering.
4. High Accuracy – 96.88% training and 87.52% validation accuracy on DME datasets.
5. Consistency Mechanism – Maintains stable responses across similar medical queries.
6. Lightweight & Interpretable – Simplified fusion pipeline ensures computational efficiency.

Methodology
1. Data Preprocessing

Images resized to 448×448 pixels and standardized for VGG16 input.

Text questions tokenized, embedded via Word2Vec (300-D), and padded to 40 tokens.

2. Feature Extraction

VGG16 extracts high-level spatial features from fundus images.

LSTM processes question sequences to capture contextual semantics.

3. Feature Fusion

Late fusion (concatenation) merges image and text features for unified representation.

4. Training

Optimized with Adam, categorical cross-entropy, and ReduceLROnPlateau callbacks.

Output layer uses Softmax for 476 answer categories.

Results
|          Metric         | Accuracy |
| :---------------------: | :------: |
|  **Training Accuracy**  |  96.88%  |
| **Validation Accuracy** |  87.52%  |

Outperformed ResNet101 in DME grading tasks.

Provided consistent answers to related medical questions.

Ensured reliable interpretations for fundus image analysis.

Dataset
Sources:

IDRiD Dataset
eOphta Dataset
Includes 433 training images with 9779 question–answer pairs, focusing on DME grading and hard exudate detection.

Technologies Used

Programming: Python

Frameworks: TensorFlow, Keras

Libraries: NumPy, Pandas, Matplotlib, NLTK

Models: VGG16, Word2Vec, LSTM

Tools: Jupyter Notebook, PowerPoint (for visualization)

Insights

The model accurately grades Diabetic Macular Edema from retinal images.

Demonstrates human-like logical reasoning without predefined rules.

Balances accuracy, consistency, and interpretability, crucial for medical AI applications.

Future Scope

Integrate Transformer-based architectures (e.g., ViT, BERT) for advanced reasoning.

Introduce formal consistency metrics for reliability evaluation.

Extend the framework to other medical imaging modalities like MRI and CT.

Impact

This research contributes to AI-driven healthcare by empowering diagnostic systems with interpretable, multimodal intelligence. The proposed VQA model demonstrates the potential of combining vision and language for automated, trustworthy clinical support — a crucial step toward AI-assisted precision medicine.

Authors

Pragatilaxmi Itigowni – Model Design, Data Analysis, and Documentation

Khushi Chalageri, Disha Kalyanshettar, Saakshi Lokhande, Vaishnavi Ajjevadeyarmath

Under Guidance of: Prof. Channabasappa Muttal

Institution: School of Computer Science and Engineering, KLE Technological University, Hubballi
