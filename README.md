# Helmet-Detection-using-YOLOv5

YOLO an acronym for 'You only look once' is an object detection algorithm that divides images into a grids.Each cell in the grid is responsible for detecting objects within itself.

YOLO is one of the most famous object detection algorithms due to its speed and accuracy.

YOLO V5

MODEL ARCHITECTURE

Yolo v5 is a single--stage object detector.

It has three important parts
    Model backbone
    Model Neck
    Model Head

    Model backbone is used for feature extraction.It extracts important features from given input image.CSP-Cross
Stage Partial Networks are used as a backbone in yolo v5.

    Model Neck is used to generate feature pyramids.Feature pyramids help model to generalize.Feature model helps
model to perform well on unseen data.In yolo v5 Path Aggregation Network[panet] is used as neck to get feature pyramids.
 
    Model Head is used to perform final detection.It applies anchor boxes on features and generates final output
vectors with class probabilites,objectness score,bounding boxes.



ACTIVATION FUNCTION

    YOLO v5 uses ReLU[rectified linear activation function] and Sigmoid activation function.
    
    In YOLO v5 the Leaky ReLU activation function is used in middle/hidden layers and the sigmoid activation
function is used in the final detection layer.


OPTIMIZATION FUNCTION

    In YOLO v5,the default optimization function for training is Stochastic Gradient Descent (SGD).
    
    We can change it to Adam.


COST FUNCTION
    
    In YOLO family, the compound loss is calculated based on objectness score, class probability score and bounding box regression score.
    
    Ultralytics have used Binary Cross-Entropy with Logits Loss function from PyTorch for loss calculation of class probability and object score.
