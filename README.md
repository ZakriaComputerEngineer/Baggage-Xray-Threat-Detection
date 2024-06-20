# Baggage-Xray-Threat-Detection

Flowchart:

CLASSIFICATION




















SEGMENTATION





















CLASSIFICATION
For classifying between the three classes (safe, gun, knives) I’ve used a CNN model Resnet18 which contains 18 conv layers with 11M trainable parameters suitable for this job. Here is the complete of the model on dummy input (3,256,256). Dataset loading is done on batch size 4 after which this is the images and mask in one batch:
  
 
 
 
 

I’ve made a predictions csv file for predictions data and true labels side by side:
 

SEGMENTATION
For segmentation I’ve used the lab provided WNET model architecture code and organized the dataset in this format for semantic segmentation.












   
 
 
 PREDICTED_IMAGES 
F1 SCORE
 
UNET (COMPARISON):
My previous work on this same dataset I used unet to implement semantic segmentaion. UNET provided accuracy/F1 61%. Both models seems to work fine in isolated object’s Xrays but complete baggage Xrays seems to become a problem for these kind of small models.










WNET				           UNET				TRUE

