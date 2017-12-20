~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
###Result 1:
Dataset Used: MIT CBCL
Algorithm used: ConvNet (2 conv layers: W1 [4,4,1,8], W2 [2,2,8,16], 50 epochs, 32 mini batch)
Program file: ConvNet.py

Cost after epoch 0: 0.637132
Cost after epoch 5: 0.000197
Cost after epoch 10: 0.000053
Cost after epoch 15: 0.000022
Cost after epoch 20: 0.000012
Cost after epoch 25: 0.000007
Cost after epoch 30: 0.000004
Cost after epoch 35: 0.000003
Cost after epoch 40: 0.000002
Cost after epoch 45: 0.000001
Tensor("Mean_1:0", shape=(), dtype=float32)
Train Accuracy: 1.0
Test Accuracy: 0.100198

Improvements: horrendously overfitting
Model saved as: not saving
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
###Result 2:
Dataset Used: MIT CBCL (Train only), randomized 50% holdout validation
Algorithm used: ConvNet (2 conv layers: W1 [3,3,1,8], W2 [3,3,8,16], 50 epochs, 32 mini batch) 
Program file: Result2/ConvNet.py

Cost after epoch 0: 0.517286
Cost after epoch 5: 0.000205
Cost after epoch 10: 0.000083
Cost after epoch 15: 0.000047
Cost after epoch 20: 0.000030
Cost after epoch 25: 0.000021
Cost after epoch 30: 0.000015
Cost after epoch 35: 0.000012
Cost after epoch 40: 0.000009
Cost after epoch 45: 0.000007
Tensor("Mean_1:0", shape=(), dtype=float32)
Accuracy: 1.0

Improvements: None - Perfect Accuracy, try with more layers for better deconvolutional understanding
Parameters saved as: Result2/params.pckl
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
###Result 3:
Dataset Used: Yale B, randomized 50% holdout validation
Algorithm used: ConvNet (2 conv layers: W1 [3,3,1,8], W2 [3,3,8,16], 50 epochs, 32 mini batch) 
Program file: Result3/ConvNet.py

Cost after epoch 0: 0.334250
Cost after epoch 5: 0.000231
Cost after epoch 10: 0.000057
Cost after epoch 15: 0.000033
Cost after epoch 20: 0.000015
Cost after epoch 25: 0.000007
Cost after epoch 30: 0.000005
Cost after epoch 35: 0.000004
Cost after epoch 40: 0.000003
Cost after epoch 45: 0.000002
Tensor("Mean_1:0", shape=(), dtype=float32)
Accuracy: 0.999321

Improvements: None - Close to Perfect Accuracy, try with more layers for better deconvolutional understanding
Parameters saved as: Result3/params.pckl
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
###Result 4:
Dataset Used: Yale B, randomized 50% holdout validation
Algorithm used: ConvNet (4 conv layers: W1 [3,3,1,8], W2 [3,3,8,16], W3[3,3,16,32], W4[3,3,32,32] 50 epochs, 32 mini batch) 
Program file: Result4/ConvNet.py

Cost after epoch 0: 0.687914
Cost after epoch 5: 0.008760
Cost after epoch 10: 0.000467
Cost after epoch 15: 0.000408
Cost after epoch 20: 0.000375
Cost after epoch 25: 0.000345
Cost after epoch 30: 0.000313
Cost after epoch 35: 0.000278
Cost after epoch 40: 0.000242
Cost after epoch 45: 0.000204
Tensor("Mean_1:0", shape=(), dtype=float32)
Accuracy: 0.997622

Improvements:Close to Perfect Accuracy, increasing layers hurt accuracy. look at other CNN architechtures and see what's wrong
Parameters saved as: Result4/params.pckl
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
###Result 5:
Dataset Used: MIT CBCL (Train only), randomized 50% holdout validation
Algorithm used: ConvNet (4 conv layers: W1 [3,3,1,8], W2 [3,3,8,16], W3[3,3,16,32], W4[3,3,32,32] 50 epochs, 32 mini batch) 
Program file: Result5/ConvNet.py

Cost after epoch 0: 0.801217
Cost after epoch 5: 0.000152
Cost after epoch 10: 0.000052
Cost after epoch 15: 0.000028
Cost after epoch 20: 0.000018
Cost after epoch 25: 0.000012
Cost after epoch 30: 0.000009
Cost after epoch 35: 0.000007
Cost after epoch 40: 0.000005
Cost after epoch 45: 0.000004
Tensor("Mean_1:0", shape=(), dtype=float32)
Accuracy: 1.0

Improvements: None - Perfect Accuracy, increasing layers didnt affect accuracy. look at other CNN architechtures and try 
Parameters saved as: Result5/params.pckl
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
###Result 6:
Dataset Used: Yale B, randomized 50% holdout validation
Algorithm used: ConvNet (4 conv layers: W1 [3,3,1,8], W2 [3,3,8,16], W3[3,3,16,32], W4[3,3,32,32], 2 FC layer:(FC1: 1024 neurons with dropout = 0.4, FC2: 10 neurons for 10 classes), 50 epochs, 32 mini batch) 
Program file: Result6/ConvNet.py

Cost after epoch 0: 0.688742
Cost after epoch 5: 0.015282
Cost after epoch 10: 0.006424
Cost after epoch 15: 0.004764
Cost after epoch 20: 0.000030
Cost after epoch 25: 0.000014
Cost after epoch 30: 0.000008
Cost after epoch 35: 0.000005
Cost after epoch 40: 0.000003
Cost after epoch 45: 0.000002
Tensor("Mean_1:0", shape=(), dtype=float32)
Accuracy: 0.997962

Improvements:Close to Perfect Accuracy, marginal increase in accuracy but cost function is getting lower. Try with different filter sizes.
Parameters saved as: Result6/params.pckl

