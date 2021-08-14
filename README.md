# kinship-recognition
siamese network using transfer learning on resnet50 and vgg16, binary classification.  
one input sample to this network consists of one or many images of the two people being compared.  
v1: base. 0.51800.  
v2: changing last 10 layers.  0.52666.  
v3: only concatenating layers (without top), adding dense layers and dropout regularization, adding methods of combining networks --> all nominal. keep fine tuning last three layers.   
v4: changed combination of inputs. 0.53866 (retry for final v, 50min training).  
v5: 60 epochs. 0.51 --> model is not underfitting (keep at 25).  
