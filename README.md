# Animal Classification Model Original (Alpha_Final_3) vs (Alpha_5)
This repository contains an animal classification model that can identify 10 different animal classes from images.

## Model Evolution
### Original Model
The original animal classification model was developed as a baseline solution with the following characteristics:

- **Architecture**: Basic CNN with standard convolutional and pooling layers
- **Training Data**: Dataset of 10 animal classes with limited augmentation
- **Performance**:
  - Training Accuracy: ~95.2%
  - Validation Accuracy: ~82.7%
- **Limitations**:
  - Overfitting on training data
  - Limited generalization to new images
  - Confusion between visually similar classes (e.g., dog/cat, butterfly/spider)

### Improved Model (Alpha 5)
The Alpha 5 model represents a significant improvement over the original model:

- **Architecture**: 
  - Improved CNN architecture with deeper layers
  - Custom layers with residual connections
  - Batch normalization for better training stability
  - Dropout layers to reduce overfitting
  
- **Training Improvements**:
  - Enhanced data augmentation (rotation, zoom, flip, shift)
  - Learning rate scheduling
  - Early stopping to prevent overfitting
  
- **Performance**:
  - Training Accuracy: ~99.05%
  - Validation Accuracy: ~88.40%
  
- **Key Advantages**:
  - Better generalization to unseen images
  - Reduced confusion between similar classes
  - Faster inference time
  - More robust feature extraction
    
### Using EfficentNetB6 transfer model
  - High Accuracy:
The model achieved a validation accuracy of approximately 91-92% after 10 epochs.
  - Strong F1-Scores:
Demonstrated strong performance with a Macro F1-Score of approximately 0.9087 and a Weighted F1-Score of approximately 0.9178, indicating balanced precision and recall across all animal classes.
  - Effective Transfer Learning:
Utilized EfficientNetB6 pre-trained on ImageNet. The base model layers where frozen.
  - Robust Classification:
The classification report and confusion matrix reveal high precision and recall for most animal categories, with some minor variations.
