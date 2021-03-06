# camvid
 
	Please cite: 	
	

	
	(1)
	Segmentation and Recognition Using Structure from Motion Point Clouds, ECCV 2008 (pdf)
Brostow, Shotton, Fauqueur, Cipolla (bibtex)

	
	(2)
	Semantic Object Classes in Video: A High-Definition Ground Truth Database (pdf)
Pattern Recognition Letters (to appear)
Brostow, Fauqueur, Cipolla (bibtex)

	
	
	

	Description:
	  
	The Cambridge-driving Labeled Video Database (CamVid) is the first collection of videos with object class semantic labels, complete with metadata. The database provides ground truth labels that associate each pixel with one of 32 semantic classes.

The database addresses the need for experimental data to quantitatively evaluate emerging algorithms. While most videos are filmed with fixed-position CCTV-style cameras, our data was captured from the perspective of a driving automobile. The driving scenario increases the number and heterogeneity of the observed object
classes.

Over ten minutes of high quality 30Hz footage is being provided, with corresponding semantically labeled images at 1Hz and in part, 15Hz. The CamVid Database offers four contributions that are relevant to object analysis researchers. First, the per-pixel semantic segmentation of over 700 images was specified manually, and was then inspected and confirmed by a second person for accuracy. Second, the high-quality and large resolution color video images in the database represent valuable extended duration digitized footage to those interested in driving scenarios or ego-motion. Third, we filmed calibration sequences for the camera color response and intrinsics, and computed a 3D camera pose for each frame in the sequences. Finally, in support of expanding this or other databases, we offer custom-made labeling software for assisting users who wish to paint precise class-labels for other images and videos. We evaluated the relevance of the database by measuring the performance of an algorithm from each of three distinct domains: multi-class object recognition, pedestrian detection, and label propagation.

## 11-class CamVid dataset (SegNet)

The 11-class version of CamVid is a popular benchmark in semantic segmentation. The authors of [SegNet](http://mi.eng.cam.ac.uk/projects/segnet/) have made available a [version](https://github.com/alexgkendall/SegNet-Tutorial/tree/master/CamVid) of this dataset but with downsampled images (480x360). The following helper files contain relevant information to transform the raw images and labels, at a resolution of 960x768, in a dataset similar to the one used on SegNet:

- ``segnet_class_map``: 32 class to 11 class mapping;
- ``segnet_colors``: color codes for each of the 11 classes;
- ``segnet_test``: filenames of the images that belong to the test dataset as established on [SegNet](https://github.com/alexgkendall/SegNet-Tutorial/tree/master/CamVid);
- ``segnet_train``: filenames of the images that belong to the training dataset as established on [SegNet](https://github.com/alexgkendall/SegNet-Tutorial/tree/master/CamVid);
- ``segnet_val``: filenames of the images that belong to the validation dataset as established on [SegNet](https://github.com/alexgkendall/SegNet-Tutorial/tree/master/CamVid);
