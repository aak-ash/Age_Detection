## Pre-Processing

Resizing the input to 28*28 which is then given as input to model

## Data -Info 
Classes 3 : Middle , Young , Old </br> 
Converted to One-Hot Vector before using 

## Architecture Used 
* Convolution(3,20,5,1) + Relu
* Max_Pool with Stride : 2 and Kernel size :2 
* Batch_Normalisation
* Convolution(20,50,5,1) + Relu
* Convolution(50,60,5,1) + Relu
* Max_Pool with Stride : 2 and Kernel size :2 
* Unravel (2*2*60 -> 500) + Relu
* Linear (500 -> 10) +Relu
* Linear (10 -> 3)
* CrossEntropyLoss 

## Optimizer

Stochastic with Momentum is used </br> 
Momentum = 0.9 </br> 
Learning_rate =0.01 </br> 

## Results 

Number_epoch : 2    Accuracy : 60.43% </br> 
Number_epoch : 10   Accuracy : 73.55% </br> 
Number_epoch : 30   Accuracy : 81.21% </br> 



