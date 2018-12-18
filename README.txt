For the CIFAR-10 dataset,

Number of training points : 1000
Number of testing points : 500
Number of validation points : 300

On account of time constraints and training issues of a large dataset, I was only able to train on a subset of images for CIFAR-10 dataset.
Epochs on which the model was trained on ~ 20 epochs on HPC.

Baseline AlexNet model: 
	Training logs can be found in pure_alexnet.txt
	Test Accuracy: 0.22
	Final Loss: 5.3069339

Concat_CP Alexnet model:
	Training logs can be found in concat_cp.txt
	Test Accuracy: 0.4700
	Final Loss: 2.3174005

Concat_DP Alexnet model:
	Training logs can be found in concat_dp.txt
	Test Accuracy: 0.28
	Final Loss: 2.6470273

Indep_CP Alexnet model:
	Training logs can be found in indep_dp.txt
	Test Accuracy: 0.45
	Final Loss: 2.6794

Indep_DP Alexnet model:
	Training logs can be found in indep_dp.txt
	Test Accuracy: 2.574
	Final Loss: 0.21

Using the idea of attention maps, we can see the trend in the values of test accuracy which is greater than baseline model.

Attention Maps can be found under the images folder where we can see the attention values giving importance to the objects in the image, and hence causing the increase in the accuracy.
