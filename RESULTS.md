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
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
###Result 7:
Dataset Used: Yale B, randomized 50% holdout validation
Algorithm used: ConvNet (4 conv layers: W1 [3,3,1,8], W2 [5,5,8,16], W3[5,5,16,32], W4[3,3,32,32], 2 FC layer:(FC1: 1024 neurons with dropout = 0.4, FC2: 10 neurons for 10 classes), 50 epochs, 32 mini batch) 
Program file: Result7/ConvNet.py

Cost after epoch 0: 0.615710
Cost after epoch 5: 0.083954
Cost after epoch 10: 0.013602
Cost after epoch 15: 0.004772
Cost after epoch 20: 0.000148
Cost after epoch 25: 0.000022
Cost after epoch 30: 0.000009
Cost after epoch 35: 0.000005
Cost after epoch 40: 0.000003
Cost after epoch 45: 0.000002
Tensor("Mean_1:0", shape=(), dtype=float32)
Accuracy: 0.998291

Improvements:Close to Perfect Accuracy, marginal increase in accuracy but cost function is getting lower. going to further increase filter size and start with UMist dataset
Parameters saved as: Result7/params.pckl
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
###Result 8:
Dataset Used: Yale B, randomized 50% holdout validation
Algorithm used: ConvNet (4 conv layers: W1 [5,5,1,8], W2 [5,5,8,16], W3[5,5,16,32], W4[5,5,32,32], 2 FC layer:(FC1: 1024 neurons with dropout = 0.4, FC2: 10 neurons for 10 classes), 50 epochs, 32 mini batch) 
Program file: Result7/ConvNet.py (just change 3x3 to 5x5 in all)

Cost after epoch 0: 1.116897
Cost after epoch 5: 0.032055
Cost after epoch 10: 0.012570
Cost after epoch 15: 0.035283
Cost after epoch 20: 0.000905
Cost after epoch 25: 0.000746
Cost after epoch 30: 0.000749
Cost after epoch 35: 0.000752
Cost after epoch 40: 0.000749
Cost after epoch 45: 0.000740
Tensor("Mean_1:0", shape=(), dtype=float32)
Accuracy: 0.998291

Improvements:Close to Perfect Accuracy, no increase in accuracy but cost function is getting higher.
Parameters saved as: Result8/params.pckl
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
###Result 9:
Dataset Used: UMIST, randomized 50% holdout validation
Algorithm used: ConvNet (4 conv layers: W1 [5,5,1,8], W2 [5,5,8,16], W3[5,5,16,32], W4[5,5,32,32], 2 FC layer:(FC1: 1024 neurons with dropout = 0.4, FC2: 10 neurons for 10 classes), 50 epochs, 32 mini batch) 
Program file: Result9/ConvNet.py

Cost after epoch 0: 1.454234
Cost after epoch 5: 1.020982
Cost after epoch 10: 0.674410
Cost after epoch 15: 0.492433
Cost after epoch 20: 0.243030
Cost after epoch 25: 0.128847
Cost after epoch 30: 0.157627
Cost after epoch 35: 0.058738
Cost after epoch 40: 0.058883
Cost after epoch 45: 0.009984
Tensor("Mean_1:0", shape=(), dtype=float32)
Accuracy: 0.82

Improvements:Low Accuracy, train longer
Parameters saved as: Result9/params.pckl
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
###Result 10
Dataset Used: UMIST, randomized 50% holdout validation
Algorithm used: ConvNet (4 conv layers: W1 [5,5,1,8], W2 [5,5,8,16], W3[5,5,16,32], W4[5,5,32,32], 2 FC layer:(FC1: 1024 neurons with dropout = 0.4, FC2: 10 neurons for 10 classes), 75 epochs, 32 mini batch) 
Program file: Result9/ConvNet.py

Cost after epoch 0: 1.452676
Cost after epoch 5: 0.952903
Cost after epoch 10: 0.714621
Cost after epoch 15: 0.314862
Cost after epoch 20: 0.225411
Cost after epoch 25: 0.055632
Cost after epoch 30: 0.107403
Cost after epoch 35: 0.082473
Cost after epoch 40: 0.035992
Cost after epoch 45: 0.004037
Cost after epoch 50: 0.000126
Cost after epoch 55: 0.000090
Cost after epoch 60: 0.000073
Cost after epoch 65: 0.000061
Cost after epoch 70: 0.000052
Tensor("Mean_1:0", shape=(), dtype=float32)
Accuracy: 0.88

Improvements:Low Accuracy, train longer
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
###Result 11
Dataset Used: UMIST, randomized 50% holdout validation
Algorithm used: ConvNet (4 conv layers: W1 [5,5,1,8], W2 [5,5,8,16], W3[5,5,16,32], W4[5,5,32,32], 2 FC layer:(FC1: 1024 neurons with dropout = 0.4, FC2: 21 neurons for 21 classes), 120 epochs, 32 mini batch) learning rate = 0.003
Program file: Result11/ConvNet.py

Cost after epoch 0: 1.428947
Cost after epoch 5: 1.030099
Cost after epoch 10: 0.519338
Cost after epoch 15: 0.207566
Cost after epoch 20: 0.331442
Cost after epoch 25: 0.102161
Cost after epoch 30: 0.030378
Cost after epoch 35: 0.067521
Cost after epoch 40: 0.026794
Cost after epoch 45: 0.099165
Cost after epoch 50: 0.058770
Cost after epoch 55: 0.001918
Cost after epoch 60: 0.000388
Cost after epoch 65: 0.000258
Cost after epoch 70: 0.000192
Cost after epoch 75: 0.000148
Cost after epoch 80: 0.000117
Cost after epoch 85: 0.000095
Cost after epoch 90: 0.000079
Cost after epoch 95: 0.000067
Cost after epoch 100: 0.000057
Cost after epoch 105: 0.000050
Cost after epoch 110: 0.000044
Cost after epoch 115: 0.000039
Tensor("Mean_1:0", shape=(), dtype=float32)
Accuracy: 0.975

Improvements:Low Accuracy, train longer
Parameters saved as: Result11/params.pckl
