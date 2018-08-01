# Medico: The 2018 Multimedia for Medicine Task 

## Task Description
The Medico Task tackles the challenge of predicting diseases based on multimedia data collected in hospitals with two additional requirements: perform the analysis efficiently (i.e., minimize processing time) and use as little data as possible for training. As an additional, exploratory, subtask, participants are asked to generate automatic text reports (summaries) of the findings. 

For the task, we will provide a large dataset of at least nine different findings in the human GI tract containing videos and images (at least 1000 images per class for training and test set). The data will be split into different parts for cross validation. The ground truth for the data is collected from medical experts (specialists in GI endoscopy), who annotate the images and videos.

Based on this data, the participants will be asked to solve four subtasks (two main tasks and two optional tasks):

1. ***Classification of diseases and findings***. Design and implement classifiers to predict the annotations of medical experts.
2. ***Fast and efficient classification***. Design and implement a classifier that minimize that minimize the processing time and also the training data requirements.
3. ***Basic Reporting*** (exploratory/optional). Summarization of a video in terms of how many different diseases and findings have occurred. For example, if the same polyp occurs twice it should only be counted one time for the summary.
4. ***Advanced reporting*** (exploratory/optional). Automatically create a text-report for a physician for three video cases. When the task data is released, we will provide some examples, and a detailed description of what the medical experts do with the report (a definition of what a text report is and what should capture and how).

The dataset is publicly available for participants and other multimedia researchers without any restriction.

## Task motivation
In some areas of the human body, such as the GI tract, which is the focus of this task, the detection of abnormalities and diseases in early stages can significantly improve the chance of successful treatment and survival. Through endoscopic examinations (insertion of a camera in for example the GI tract), diseases can be detected visually, even before they become symptomatic. This is particularly important for cancers of the large bowel (colorectal cancer) or cancer-precursors (colorectal polyps), which can be detected through colonoscopy or capsule endoscopy. 

The task differs from other well-known medical imaging tasks, such as the ImageClef medical tasks, in that it (i) uses multimedia data (videos and images) and not medical imaging data (CT scans, etc.), (ii) requires using as little training data as possible and (iii) evaluates the approaches also regarding processing time. 

We hope that this task will encourage the multimedia community to help to improve the healthcare system through application of their knowledge and methods to reach the next level of computer and multimedia assisted diagnosis, detection and interpretation of abnormalities. In previous research in this area, computer vision and medical imaging have created visual augmentations of the interior of a body. To automatically detect and locate abnormalities visual representations this technology is not sufficient. There is a need for efficient and effective image and video processing, analysis, information retrieval, and systems which integrate the expertise of medical experts. This need is the motivation behind the Medico Task.

## Target group
The task is of interest to researchers in the areas of machine learning (classification), visual content analysis and multimodal fusion. Overall, this task is intended to encourage the multimedia community to help improve the health care system through application of their knowledge and methods to reach the next level of computer and multimedia assisted diagnosis, detection and interpretation of abnormalities. 

## Data
Overall, the dataset will contain a multi-class set of frames and videos for at least 4 different diseases, at least 4 different landmarks and at least 2 different findings. Each class will consist of at least 1000 frames and at least 2 short videos. The training set will be released with ground truth. All the frames in training set will be labelled with corresponding class-label. Up to 10% of training set frames will have a detailed ground truth masks showing the exact location of disease or finding within the frame. The ground truth is collected with the help of GI endoscopists from our partner hospitals. We will also provide pre-extracted visual features for all data. 

## Ground truth and evaluation
1. Classification of diseases and findings: The evaluation metric is the multiclass version of the Mathews Correlation Coefficient, which captures the quality of classification as reflected in the correlation between the ground truth and the classifier's predictions. 
2. Fast and efficient classification: For the evaluation, the participants are asked to run the code on a standard PC and provide information about hardware used. The time from input to output will be measured and weighed by the accuracy of the output. Participants are also asked to record the amount of training data used. The amount of training data will also be weighted by the accuracy of the output.
3. Basic Reporting (exploratory/optional): The metric will reflect the completeness and the correctness of the summary. This subtask allows us to focus on understanding the performance of the automatic systems in practice (from the point of view of the medical expert).
4. Advanced reporting (exploratory/optional): This subtask will be assessed manually from two of our medical partners in terms of how useful it is for them and if it satisfies existing demands for documentation of endoscopic procedures. The assessment will follow a list of requirements that will be provided to the participants before they submit their results.

## Recommended reading
> [1] Pogorelov, Konstantin, et al. "Kvasir: a multi-class image dataset for computer aided gastrointestinal disease detection." Proceedings of the 8th ACM Multimedia Systems Conference. ACM, 2017.  
> [2] Riegler, Michael, et al. "Multimedia and Medicine: Teammates for Better Disease Detection and Survival." Proceedings of the 2016 ACM Multimedia Conference. ACM, 2016.  
> [3] Y. Wang, W. Tavanapong, J. Wong, J. Oh, and P. C. de Groen. Computer-aided detection of retroflexion in colonoscopy. In Proc. of CBMS, pages 1–6, 2011.  
> [4] Y. Wang, W. Tavanapong, J. Wong, J. H. Oh, and P. C. de Groen. Polyp-alert: Near real-time feedback during colonoscopy. Computer methods and programs in biomedicine, (3), 2015.  

We recommend also having a look at the last year’s task papers in the MediaEval 2017 Proceedings:
> Guillaume Gravier et al. (eds.) 2017. Proceedings of the MediaEval 2017 Workshop, Dublin, Ireland, Sept. 13-15, 2017.

## Task organizers
- Konstantin Pogorelov, Simula Research Laboratory & University of Oslo, Norway konstantin at simula.no
- Michael Riegler, Simula Research Laboratory & University of Oslo, Norway michael at simula.no
- Pål Halvorsen, Simula Research Laboratory & University of Oslo, Norway
- Thomas de Lange, Cancer Registry of Norway, Norway
- Kristin Ranheim Randel, Cancer Registry of Norway, Norway
- Duc-Tien Dang-Nguyen, Dublin City University, Ireland
- Mathias Lux, University of Klagenfurt, Austria mlux at itec.aau.at
