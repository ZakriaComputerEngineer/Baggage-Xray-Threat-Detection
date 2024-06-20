# Baggage-Xray-Threat-Detection

CLASSIFICATION
For classifying between the three classes (safe, gun, knives) I’ve used a CNN model Resnet18 which contains 18 conv layers with 11M trainable parameters suitable for this job. Here is the complete of the model on dummy input (3,256,256). Dataset loading is done on batch size 4 after which this is the images and mask in one batch:
 ![image](https://github.com/ZakriaComputerEngineer/Baggage-Xray-Threat-Detection/assets/150436890/f3db4a70-20c9-48e7-b4ed-04e1d6a72aa5)

 ![image](https://github.com/ZakriaComputerEngineer/Baggage-Xray-Threat-Detection/assets/150436890/f02022e3-a009-4fc0-9d24-7d502fcbc4a9)

 ![image](https://github.com/ZakriaComputerEngineer/Baggage-Xray-Threat-Detection/assets/150436890/94c65603-1858-45fd-a01d-967fda4d1833)

SEGMENTATION
For segmentation I’ve used the lab provided WNET model architecture declared through code having 32 conv layers and organized the dataset in this format for semantic segmentation.

root_dataset_folder/
│
├── train/
│   ├── images/
│   │   ├── img1.jpg
│   │   └── ...
│   ├── gt/
│   │   ├── mask1.png
│   │   └── ...
├── test/
│   ├── images/
│   │   ├── img1.jpg
│   │   └── ...
│   ├── gt/
│   │   ├── mask1.png
│   │   └── ...


![image](https://github.com/ZakriaComputerEngineer/Baggage-Xray-Threat-Detection/assets/150436890/3dd12826-34e2-402d-8bc9-5c61f700deb4)
![image](https://github.com/ZakriaComputerEngineer/Baggage-Xray-Threat-Detection/assets/150436890/0122127f-7bb0-409f-8dd7-be88c696118c)

 PREDICTED_IMAGES
 ![image](https://github.com/ZakriaComputerEngineer/Baggage-Xray-Threat-Detection/assets/150436890/4c3c721f-db50-4895-b3af-621e2f8171f5)

 F1 SCORE
 ![image](https://github.com/ZakriaComputerEngineer/Baggage-Xray-Threat-Detection/assets/150436890/28b30535-647f-41a9-847d-032719987116)

 







