# Kinship-Recognition
Single and double siamese networks using combinations of transfer-learned ResNet50, VGG16, and FaceNet for kinship recognition.  
An input to these networks consist of one or many images of the two people being compared.  

### ResNet50 ###
v1: Resnet50: 0.51800.  
v2: changing last 10 layers: 0.52666.  
v3: only concatenating layers (freeze all weights, no top), adding dense layers and dropout regularization, adding methods of combining networks --> all nominal.     
v4: changed combination of inputs: 0.53866 (retry for final v, 50min training).  
v5: 60 epochs: 0.51 --> model is probably overfitting (keep at 25).   

### FaceNet ###
v6: FaceNet only: 0.54  

### VGG16 ###
v7: VGG16 only: 0.56  

### FaceNet and VGG16 ###
v8: double siamese FaceNet and VGG16: 0.52  

### ResNet50 and VGG16 ###
v9: double siamese ResNet50 and VGG16 without robust generator: 0.56  
v10: double siamese VGG16 and ResNet50: 0.55  
