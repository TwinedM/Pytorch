Torch (2002)
could do tensor based operations which could make cnn and rnns 
Probelems
- It was a Lua based framework (was built in lua programming lang)
- computation graph was static
- new library but in python is Pytorch


Ver 1.0
Benefits of Pytorch
- compatibility 
- Dynamic computation graph - visual way of representing maths in forms of graphs
    graph can be changed in runtime (especially experimentation)

TorchScript - serialization allows the model to run without any python or pytorch (good in app dev web dev etc etc)
Caffe2 - deep learning lib for scalable models , used in production (this was merged in pytorch)

Distributed training support 
ONNX compatibilty (open neural network exchange) - ONNX format model can be used in other libraries too
Quantization support - rather than storing weights in floats we use int ( use a datatype that takes less space) - this makes the model small
Ecosystem libs - torchvision,torchtext,torchaudio

Pytorch Lightning - high level api for pytroch
Hugging Face Transformers
Cloud support too

Ver 2.0
Mainly Optimisation

Latency improvements
Throughput - how much data can be processed at once

CORE FEATURES
- Tensor Computations 
- GPU Accel
- Dynamic Computation Graph
- Automatic Differentiation - autograd
- Distributed Training
- Interoperability with other libs


Tensors in pytorch

 These tensors are very efficient and also parallely especially in GPU and TPU
 
 Where are they used 
    Data storage 
    Weights and Biases : the learnable parameters of neural network 
    Matrix Operations
    Training Process
 



VIDEO # 3 

AUTOGRAD 
Need of autograd
Coding functions of nested functions is very difficult hence we use autograd
It enables gradient computation, which is essential for training ml models using optimisation algo like gradient descent.
For more info go to Tensors.ipynb


VIDEO #4 
TRAINING PIPELINE

Dataset -> NN AIM - For training pipeline
Dataset - breast cancer
Read the code for better one
1) W new  = Wold - Learning rate * DL/DW
2) Dont update the params without using with no_grad
3) Always reset the grads 
4) retain graph - holds the intermediate values too

VIDEO #5
NN module automate all the stuff i did in last lecture
1) The conversion from numpy array to tensor is of float64 data type but the nn module does calcs at float 32 


VIDEO #6 
Dataset and DataLoader

Why?
Flaw in code 
We are using batch gradient descent ie we are using all the data single time mai hi 
as it is memory inefficient
Convergence value is not good (the updates are not as fast)





