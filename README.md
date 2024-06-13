# Content Extraction from Product Images: A System for Sticker Segmentation and Classification

Automatic image processing techniques play a crucial role in various applications, including object detection and classification. This project presents a system for segmenting, localizing, and unsupervised classification of stickers within grayscale images. The system addresses the challenge of separating and identifying stickers without relying on pre-labeled data.

The **segmentation** leverages a modified 3-level Otsu's thresholding method, separating the image into distinct regions for printed content, sticker background, and cardboard background. 

**Localization** utilizes contour analysis to identify rotated bounding boxes encompassing the stickers. 

**Classification** employs a two-step approach: first, extracting Hu Moments as shape features from the identified stickers, followed by K-Means clustering to categorize the stickers into "Barcode" and "Shipping Symbol" classes based on their Hu Moment similarity. 

The proposed approach effectively separates and classifies stickers within the images without the need for manual labeling with an `100% accuracy`.
