# kinship-recognition
transfer learning with resnet-50, binary classification.  
v1: base. 0.51800.  
v2: changing last 10 layers.  0.52666.  
v3: only concatenating layers (without top), adding dense layers and dropout regularization, adding methods of combining networks --> all nominal. keep fine tuning last three layers.   
v4: changed combination of inputs. 0.53866 (retry for final v, 50min training).  

v5: batch normalization
v5: add more regularization and dense layers.  
