# Neurons-Detection-Employing-a-Deep-Convolution-Neural-Network
Neurological disorders, including neurodegenerative diseases such as Alzheimer's and brain tumors, are a leading cause of death and disability across the world. Accurate image segmentation of these cells with the help of computer vision could lead to new and effective drug discoveries to treat the millions of people with these disorders. In this paper, UNet++ (Resnet34) produces more accurate cell segmentation in challenging images such as high-resolution images and small cells. The results illustrate the improvement over the wide U-net architecture, which is a powerful architecture for medical image segmentation. Our experiments demonstrate that UNet++ with a deeply supervised encoder-decoder network achieves evaluation metrics with an average IoU of 58% and pixel accuracy of 96%. This method allows to detect the large numbers of medical cell in a short time and can be applied to automated microscope detecting system.
3.2 Experimental results 

The model is implemented with PyTorch on a GPU with 25 GB of memory. The UNet++, UNet, and Mask R-CNN are employed because their architecture is helpful for cell segmentation. The Adam optimizer is applied with an initial learning rate set to 0.001 for the hyperparameters, 4 for batch size, and 50 epochs for the training process. Moreover, the error smaller than the error threshold is chosen as the optimal coefficient for the model. Each example was evaluated using the dice loss and IoU as the metric.
In this paper, the results of UNet++ are compared with those of UNet and Mask R-CNN.

Table 2. Segmentation results in test set for UNet, Mask R-CNN, UNet++ and UNet++ without CLAHE.
Model 	IoU	Dice loss	Pixel accuracy
UNet++	
	0.58	0.27	0.96
UNet
	0.55	0.29	0.95
UNet++ without CLAHE
	0.53	0.31	0.94
Mask R-CNN	0.26	1.22	0.86
			
According to the results, UNet++ has the best generalizability. The test set’s IoU and pixel accuracy are 58% and 96%, respectively. This shows that the encode and decode networks are essential principles of neuron detection. The images below show the result of the UNet++ model detecting three different cell types.
