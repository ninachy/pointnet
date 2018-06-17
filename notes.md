### 2018.6.15 
x successfully run code for object detection
x data processing in 'provider.py'
	x datatype: h5, opened by h5py
	? 2048 point are selected by FPS (farthest point sampling) from CAD model with 10k points
	x label, with 40 class
	x data, with 2048 points
x structure of code
	x utils/tf_util: defines tf_util.2d with bn & weight decay initialization wrapped
	? models/transform_nets: define T-Net
		? what is the output dimension
		? how to update by backprop?
	x models/pointnet_cls: network for classification
	  models/pointnet_cls: without T-Net
	x train
		x parameters
		x train_one_epoch, with data augmentation
		x eval_one_epoch
		x train

### 2018。6.17
x successfully run code for part segmentation
	x submit to cluster
x data processing in 'provider.py'
	? how to convert 'PartAnnotation' to h5 data
	x 2048 points
	x label, data, seg
x structure of code
	? pointnet_part_seg: network structure (without T-Net) 
	x part_seg/train.py: training
	
	
