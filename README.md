# EnTimeMent - EU Horizon 2020 FET PROACTIVE project (2019-2022)
ENtrainment & synchronization at multiple TIME scales in the MENTal foundations of expressive gesture

### Software libraries for the study of the origin of movement (link: [Origin-of-Movement](https://github.com/EnTimeMent/Origin-of-Movement))

The software, written in Matlab, extracts movement features (speed, tangential acceleration, kinetic energy, angular momentum) for two skeleton models of the human body, which refer to two different spatial scales. Then, such features are filtered and combined to compute a dissimilarity measure for the joints, from which a transferable utility game on an auxiliary graph is constructed. Finally, the vector of Shapley values for that game is computed (for the case in which the Shapley value coincides with the weighted degree centrality) and normalized with respect to the maximum Shapley value. The software allows for the possibility of computing the Kendall correlation between different rankings of joints. Further comments can be found inside the code.

### Software libraries for the analysis of qualities of movement (link: [Analysis-Qualities-of-Movement](https://github.com/EnTimeMent/Analysis-Qualities-of-Movement))

The purpose of this software is to analyseMotion Capture data in order to calculate the joint with the maximum Shapley Value, separately for three motion features (speed, acceleration and angular momentum). The software models the human body as a weighted undirected graph, and calculates the importance of each joint in movement. A Lowpass Butterworth filter is used on the data for cleaning and processing. Each movement feature is calculated separately for each frame of each MoCap segment. Spectral clustering on the weighted graph is applied, to compute for each frame the Shapley Values of all the joints for all the movement features. It is a mixture of Python (for the data processing, filtering, motion feature calculation and results analysis) and MATLAB (for the creation of the body as a graph andfor the Shapley Value calculation).

### Synchronization among temporal scales: the MECS algorithm (link: [MECS-Algorithm](https://github.com/EnTimeMent/MECS-Algorithm))

Event Synchronization analysis was originally conceived for providing a simple and robust method to measure synchronization between two time series. This algorithm, however,and those developed as extensions thereof do not directly deal with multiple temporal scales.We extended the state-of-the-art of Event Synchronization techniquesby conceivingMulti-Event-Class Synchronization (MECS). MECS measures synchronization between events -belonging to different event classes -that are detected in multiple time series. MECS can compute synchronization between events belonging to the same class (intra-class synchronization) or to different classes (inter-class synchronization). Our technique can deal with macro-events, i.e., aggregations of events that enable analysis at multiple temporal scales.

Publication: *Volpe, G., Alborno, A., Mancini M., and Niewiadomski, R., Multi-Event-Class Synchronization (in preparation).*

### BANet machine learning architectures (link: [BANet](https://github.com/EnTimeMent/BANet))

Neural network architectures designed for automatic detection of affective behaviour from motion capture data. Detailed description of the architecture can be found in the associated publication: 

*Wang, Chongyang, Min Peng, Temitayo A. Olugbade, Nicholas D. Lane, Amanda C. De C. Williams, and Nadia Bianchi-Berthouze. "[Learning temporal and bodily attention in protective movement behavior detection.](https://ieeexplore.ieee.org/abstract/document/8925084/)" In 8th International Conference on Affective Computing and Intelligent Interaction Workshops and Demos(ACIIW), pp. 324-330. IEEE, 2019.*

<img src="https://github.com/EnTimeMent/BANet/blob/main/ACII_1.png" width="500">

### P(l)aying Attention sonification application (link: [Playing-Attention](https://github.com/EnTimeMent/Playing-Attention))

Application designed for sonification of motion capture data with respect to BAnet neural network attention weights for affectiveb ehaviour recognition from the motion capture data. Detailed description of the application can be found in the associated publication: 

*Gold, Nicolas E., Chongyang Wang, Temitayo Olugbade, N. Berthouze, and A. Williams. "[P(l)aying Attention: Multi-Modal, Multi-Temporal Music Control.](https://www.nime.org/proceedings/2020/nime2020_paper33.pdf)" In Proceedings of the International Conference on New Interfaces for Musical Expression (NIME) 2020.*

### Hierarchical HAR-PBD machine learning architectures (link: [Hierarchical_HAR-PBD](https://github.com/EnTimeMent/Hierarchical_HAR-PBD))

Neural network architectures designed for continuousdetection of affective behaviour from motion capture and muscle activity data.Detailed description of the Hierarchical HAR-PBD v1 architecture can be found in the associated publication: 

*Wang, Chongyang, Yuan Gao, Akhil Mathur, Amanda C. De C. Williams, Nicholas D. Lane, and Nadia Bianchi-Berthouze. "Leveraging activity recognition to enable protective behavior detection in continuous data." In Proceedings of the ACM on Interactive, Mobile, Wearable and Ubiquitous Technologies5, no. 2 (2021): 1-27.*

### MiMT machine learning architecture (link: [MiMT](https://github.com/EnTimeMent/MiMT))

Neural network architecture designed for automatic detection of affective behaviour at multiple timescales based on motion capture data. Detailed description of the architecture can be found in the associated publication: 

*Olugbade, Temitayo, Nicolas Gold, Amanda C. de C. Williams, and Nadia Bianchi-Berthouze. "A Movement in Multiple Time Neural Network for Automatic Detection of Pain Behaviour." In Companion Publication of the 2020 International Conference on Multimodal Interaction, pp. 442-445. 2020.*

<img src="https://user-images.githubusercontent.com/27019825/148803506-d30b59b7-9f45-4778-acc0-a3019fe09e30.png" width="500">

### huSync: Human Pose Estimation Architecture for computing Dyadic Synchronization (link: [huSync-DyadicSynchronization](https://github.com/EnTimeMent/huSync-DyadicSynchronization))

This repository contains python code to compute Dyadic Synchronization between co-performers in a small group of musicians. You will find two files:
* Module_DataExtraction: After having used AlphaPose on the video-dataset, we proceed with using this file toextract the data for each performer by isolating them individually. It stores the output as a .csv file
* Module_DyadicSynchronization: This file contains the code that extracts the data from the .csv file processed and provides the Dyadic Synchronization between all possible pairs in a musical ensemble.

Both the files have been shared as a jupyter notebook since this should make it easier to execute the code with more control. The added control helps perform experiments carefully, particularly since the data from pose estimation algorithms can be noisy and sometimes requires manual intervention.

*Sabharwal, S., Keller, P., Varlet, M., Camurri, A., Volpe, G.(2022). huSync: A novel computational approach to quantify synchronization using poseestimation algorithms - A case study assessing the effects of leadership and task structure in musical group interaction. Manuscript in preparation*

