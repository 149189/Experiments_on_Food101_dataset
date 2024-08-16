# Experiments_on_Food101_dataset
Conducted Experiments using 5 models on Food 101 Dataset

***Experiment 1***: Model_0

                      ->Data: 10 Classes of Food 101 Data (10% Training Data Only)
                      ->Pre processing: None
                      ->Model_Architecture: Feature Extraction -> EfficientNet-B0 (Pretrained on ImageNet, all layers Frozen with no top)
Accuracy: 82.68%, Loss: 0.6472

![image](https://github.com/user-attachments/assets/9b4d79f6-499d-48b1-9fb2-61d55d4c7b36)


                      
***Experiment 2 (Changes: Data-> 1% and Pre_Processing)***: Model_1 

                      ->Data: 10 Classes of Food 101 Data (1% Training Data Only)
                      ->Pre processing: Data Augmentation, Random Flips, Rotation, Zoom, Height, Width
                      ->Model_Architecture: Feature Extraction -> EfficientNet-B0 (Pretrained on ImageNet, all layers Frozen with no top)                      

Accuracy: 35.21%,  Loss: 1.8930

![image](https://github.com/user-attachments/assets/fa969478-7d1d-4f4b-9069-06dfbf65f9e8)

                  
***Experiment 3 (Changes: Data-> 10%)***: Model_2 

                      ->Data: 10 Classes of Food 101 Data (10% Training Data Only)
                      ->Pre processing: Data Augmentation, Random Flips, Rotation, Zoom, Height, Width
                      ->Model_Architecture: Feature Extraction -> EfficientNet-B0 (Pretrained on ImageNet, all layers Frozen with no top)

***Experiment 4 (Changes: Model_Architecture)***: Model_3 

                      ->Data: 10 Classes of Food 101 Data (10% Training Data Only)
                      ->Pre processing: Data Augmentation, Random Flips, Rotation, Zoom, Height, Width
                      ->Model_Architecture: Fine Tuning -> EfficientNet-B0 with top layer trained on custom data, top 10 layer unfrozen   

Experiment 5: Model_4 (Changes: Data) 

                      -> Data: 10 Classes of Food 101 Data (100% Training Data)
                      ->Pre processing: Data Augmentation, Random Flips, Rotation, Zoom, Height, Width
                      ->Model_Architecture: Fine Tuning -> EfficientNet-B0 with top layer trained on custom data, top 10 layer unfrozen                       
