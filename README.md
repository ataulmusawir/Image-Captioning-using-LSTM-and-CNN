# Image-Captioning-using-LSTM-and-CNN

### **Project Information**  
The goal of this project is to generate captions for input images by combining image and text features. The **Flickr8k dataset**, containing 8,000 images with 5 captions per image, is used. Features are extracted from images and captions, which are then merged to predict the next word in the caption sequence. The model employs **CNN** (for image features) and **LSTM** (for text features), with **BLEU Scores** used to evaluate performance.

#### **Dataset**  
- **Source**: [Flickr8k on Kaggle](https://www.kaggle.com/adityajn105/flickr8k)  
- 8,000 images and 5 captions per image.  
- Image features extracted using a pre-trained **VGG16** model.  

#### **Environment**  
- **Platform**: Kaggle  
- **Libraries Used**:  
  - numpy  
  - matplotlib  
  - keras  
  - tensorflow  
  - nltk  

#### **Neural Network Architecture**  
1. **Image Feature Extraction**:  
   - Uses **VGG16** for feature extraction.  
   - Outputs a 256-dimensional feature vector for each image.  

2. **Caption Processing**:  
   - Tokenized and padded captions processed through an **embedding layer**.  
   - LSTM layer generates sequential outputs for text processing.  

3. **Prediction**:  
   - Combines image and text features using a **CNN-LSTM network**.  
   - Outputs the next word in the caption sequence iteratively.  

#### **Evaluation**  
- **Metric**: BLEU Score  
  - **BLEU-1 Score**: 0.562067  
  - **BLEU-2 Score**: 0.373719  

This project effectively demonstrates the integration of computer vision and natural language processing to solve the image captioning problem, achieving competitive BLEU scores.
