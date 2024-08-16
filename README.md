# Experiments_on_Food101_dataset
Conducted Experiments using 5 models on Food 101 Dataset

***Experiment 1***: Model_0

                      ->Data: 10 Classes of Food 101 Data (10% Training Data Only)
                      ->Pre processing: None
                      ->Model_Architecture: Feature Extraction -> EfficientNet-B0 (Pretrained on ImageNet, all layers Frozen with no top)
Accuracy: 0.8268, Loss: 0.6472


                      
***Experiment 2 (Changes: Data-> 1% and Pre_Processing)***: Model_1 

                      ->Data: 10 Classes of Food 101 Data (1% Training Data Only)
                      ->Pre processing: Data Augmentation, Random Flips, Rotation, Zoom, Height, Width
                      ->Model_Architecture: Feature Extraction -> EfficientNet-B0 (Pretrained on ImageNet, all layers Frozen with no top)                      
                  
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
