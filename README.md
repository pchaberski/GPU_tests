# Google Colab remote GPUs vs. mobile GPU performance

Two experiments to test differences in training times between free Colab GPUs and mobile/desktop GPUs.

## GPUs tested  
- GeForce GTX 1050 Mobile (local notebook)
- GeForce GTX 1060 Desktop (local desktop)
- GeForce RTX 2060 Mobile (local notebook)
- Tesla P4 (Colab free)
- Tesla K80 (Colab free)
- Telsa T4 (Colab free)
- Tesla P100 (Colab free)

## Experiment no. 1 definition 
- task: image generation using convolutional GAN
- dataset: MNIST
- framework used: PyTorch
- 50 epochs
- [experiment notebook](https://github.com/PiotrChaberski/GPU_tests/blob/master/GAN_GPU_tests/gan_mnist_gpu_perf_test.ipynb)

## Experiment no. 1 model results
Sample of generated images and losses:  
![](https://github.com/PiotrChaberski/GPU_tests/blob/master/GAN_GPU_tests/remote_results/Tesla_P100-PCIE-16GB_20200317175444/image_at_epoch_50.png) ![](https://github.com/PiotrChaberski/GPU_tests/blob/master/GAN_GPU_tests/remote_results/Tesla_P100-PCIE-16GB_20200317175444/epoch_losses.png)

## Experiment no. 1 training times comparison
![](https://github.com/PiotrChaberski/GPU_tests/blob/master/summary_results/gan_times_summary_v3.png)

## Experiment no. 2 definition 
- task: image classification using Resnet-18
- dataset: CIFAR-100
- framework used: PyTorch
- 10 epochs
- [experiment notebook](https://github.com/PiotrChaberski/GPU_tests/blob/master/Resnet_GPU_tests/resnet_cifar100_gpu_perf_test.ipynb)

## Experiment no. 2 model results
Losses and accuracy:  
![](https://github.com/PiotrChaberski/GPU_tests/blob/master/Resnet_GPU_tests/remote_results/Tesla_P100-PCIE-16GB_20200318213725/epoch_losses.png) ![](https://github.com/PiotrChaberski/GPU_tests/blob/master/Resnet_GPU_tests/remote_results/Tesla_P100-PCIE-16GB_20200318213725/epoch_accuracy.png)

## Experiment no. 2 training times comparison
![](https://github.com/PiotrChaberski/GPU_tests/blob/master/summary_results/resnet_times_summary_v3.png)
