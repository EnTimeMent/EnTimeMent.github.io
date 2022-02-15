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

*Wang, Chongyang, Min Peng, Temitayo A. Olugbade, Nicholas D. Lane, Amanda C. De C. Williams, and Nadia Bianchi-Berthouze."Learning temporal and bodily attention in protective movement behavior detection." In 8th International Conference on Affective Computing and Intelligent Interaction Workshops and Demos(ACIIW), pp. 324-330. IEEE, 2019.*

<img src="https://github.com/EnTimeMent/BANet/blob/main/ACII_1.png" width="500">


