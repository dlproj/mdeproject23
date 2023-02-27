We have carried out the Unsupervised Monocular Depth Estimation with Left-Right Consistency POC for Resnet-18 and Resnet-50 models. The directory structure has the below distribution of files.

Readme:
This files give a detailed narrative of our experiments along with the various artifacts produced and hence the first file to be referred.

EDA:-
EDA_Kitti_Graph and EDA_Graph_CS generates the EDA for KITTI and Citiscapes dataset and EDA_KITTI_Training, EDA_KITTI_Validation and EDA_Citiscapes are saved in the Results.  MDE_EDA_Animation generates huge files and hence has not been uploaded.

Resnet18_50:-
FullRun1Debug_Monodepth.ipynb was a full run on Google Colab; it ran for 6 hours and completed 3 Epochs consuming the allocated resource.

We continued executing the project with limited set of training samples for completion purpose.
SampleDataSetup.txt has the sample data (training:validating:testing data of 80:20:20) for executing runs for Resnet-18 and Resnet-50 (Resnet18_Train_Monodepth.ipynb and Resnet50_Train_Monodepth.ipynb). The respective disparities are saved under disp18 and disp50.
MetricVisualization; compares the resnet18 and resnet50 visually. EmptyRoad and Traffic_on_Road images are available under Results.
Verify_VisualDepth; is used to visually compare the depth of both the models. TestImageWithGridLines image with grid lines is used as reference.
Verify_VisualDepth.ipynb uses the calib_cam_to_cam.txt available with the dataset to get the intrinsic parameters of the camera and we use TestImageWithGridLines to visually compare results.
MetricCalculation; calculates the various metrics for SampleDataSetup and the results are Metrices_Resnet18_50.txt

Results:-
The output of the tests .png and .txt files.  This helps to quickly get the narrative of this project.
------------------------------------------------------------------------------------------------------

List of files generated as part of the project.
------------------------------------------------------------------------------------------------------
1	Readme_Narrative		First referenc, explains the list of files
2	EDA_Graph_CS.ipynb		Citiscapes Dataset distribution
3	EDA_Kitti_Graph.ipynb		KITTI dataset distribution
4	MDE_EDA_Animation.ipynb		Code to animate the dateset scenes
5	FullRun1Debug_Monodepth.ipynb   Ran for 6 hours and exited after 3 Epochs
6	training_dirs.csv		Training Scene Data distribution csv file
7	validation_dirs.csv		Validation Scene Data distribution csv file
8	SampleDataSetup.txt		Sampling the data for the run.
9	Resnet18_Train_Monodepth.ipynb  Resnet18 with sample data
10	Resnet50_Train_Monodepth.ipynb	Resnet50 with sample data
11	MetricVisualization.ipynb	Disparities visualaton for Resnet18 and Resnet50
12	Verify_VisualDepth.ipynb	Visually check the qualitative depths for Resnet18 and Resnet50
13	MetricCalculation.ipynb		Calculating the metrics for Resnet-18 and Resnet-50
14	calib_cam_to_cam.txt		From the PyTorch implementation dataset
15	disparities.npy			Resnet18 disparity file under disp18
16	disparities_pp.npy		Resnet18 disparity file after preprocessing under disp18
17	disparities.npy			Resnet50 disparity file under disp50
18	disparities_pp.npy		Resnet50 disparity file after preprocessing  under disp50
19	EDA_KITTI_Training.png		EDA of KITTI Training data
20	EDA_KITTI_Validation.png	EDA of KITTI Validation data
21	EDA_Citiscapes.png	        EDA for Citiscapes data
22	TestImageWithGridLines.png	Test image for depth Calculation
23	EmptyRoad.png			Comparison of test image, Resnet50 and Resnet18
24	EmptyRoad_pp.png		Comparison of test image, Resnet50 and Resnet18 post processiong
25	Traffic_on_Road.png		Comparison of test image, Resnet50 and Resnet18
26	Traffic_on_Road_pp.png		Comparison of test image, Resnet50 and Resnet18 post processiong
27	Metrices_Resnet18_50.txt	Resnet-18 and Resnet-50 results comparison.

Animation of the sampled Dataset used in Resnet50_Train_Monodepth and Resnet18_Train_Monodepth:
28  2011_09_26_drive_0001_sync.mp4      Training
29  2011_09_26_drive_0020_sync.mp4      Validation and Testing
30  2011_09_26_drive_0014_sync.mp4      Other sample of the car taking the right turn
------------------------------------------------------------------------------------------------------
The Team:
Hema Aparna Medicharla, Divya Kamalasekaran, Jagadish Madhu and Arushi Rai
