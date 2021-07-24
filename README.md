# Brain Activity and Functional Connectivity during Working Memory Task

## Project for Neuromatch Academy'21 - Computational Neuroscience course

### Project Notebook

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eeCqV9JxCY2jgcivk-ftc0MZQ2WCVkfT?usp=sharing) or [Github](https://github.com/Consilium5128/NMA-BrainActivity-FC-WM/blob/main/Brain_Activity_and_FC_WM_HCP_NMA2021_BraveNeurons.ipynb)

### Project Presentation

[Google Slides](https://docs.google.com/presentation/d/1SHUJw6fKCjzev6IaG3haWjee32BIg3QRXtrBiwIAaxk/edit?usp=sharing) or [Github](https://github.com/Consilium5128/NMA-BrainActivity-FC-WM/blob/main/brave-neurons%20NMA%20project.pptx)

### Project Abstract

A principal goal of research in neuroscience is to understand and map the relationship between structure and function. Using neuroimaging tools, the neural function can be described in terms of both neural activity in certain regions/networks and functional connectivity (FC). Working memory is a cognitive function that temporarily stores information during task performance. Here, we aim to investigate brain regions that are associated with working memory and describe the neural activity and connectivity patterns of these regions among networks.

To this end, we leveraged the fMRI data from the Human Connectome Project (HCP) dataset; specifically, the task data from the n-back test, a working memory task paradigm, where participants are asked to recognize images that were just presented (0-back) or were presented two images ago (2-back). First, the average activity during the 0-back will be subtracted from the 2-back task across 360 parcels (brain regions as provided in the HCP data) to identify the regions with the highest activity. These regions should play a more significant role in working memory as verified by the statistical t-test. Second, we will compute the patterns of FC within a network consisting of the regions that show the highest activity during the working memory task. Third, we will investigate the relationship between FC and performance in the n-back task using generalized linear model logistic regression. If the timeline permits, we would expand the FC analysis to describe patterns of activity in the default mode network. 

We expect that the FC patterns within the regions with the highest neural activity during the n-back task can be used to predict task performance. Our results will expand our understanding of the neuroanatomical underpinnings of working memory and the involvement of different neural networks. This will also highlight the importance of FC measures as a functional representation. 

### Dataset

Human Connectome Project (2020) dataset as provided by Neuromatch Academy - fMRI data from 339 subjects (321 subjects for t-test and 336 for behavioral correlation with FC)

Parcellated cortical regions, 180/hemisphere (Glasser et al., 2016)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/NeuromatchAcademy/course-content/blob/master/projects/fMRI/load_hcp.ipynb) - Colab Notebook provided by Neuromatch Academy

### Working Memory Task

2 back (faces, body, tools, places) and 0 back task

For further information - [HCP Dataset Release Reference Manual](https://www.humanconnectome.org/storage/app/media/documentation/s1200/HCP_S1200_Release_Reference_Manual.pdf) or [HCP Protocols](https://www.humanconnectome.org/hcp-protocols)

### Approach for planned Analyses and Modelling

- Average activity during the 0-back was subtracted from the 2-back task across the brain regions to identify the regions with the highest activity
- Regions with the contrast analysis during working memory task was determined by contrast analysis and verified by statistical t-test using beta values from a GLM
- Networks consisting of these regions was used to compute the patterns of functional connectivity (FC) during the task
- We calculated the correlation between average FC values and performance (median response times) in the WM task

### Results

### Future Work

- Describe FC patterns within other ROIs (i.e., Default Mode Network, Multi-Modal networks) and correlate or anti-correlate with performance
- Applying approaches with higher sophistication for a better insight for predicting task performance using Functional Connectivity as well as increase robustness of analysis

### Acknowledgement

We wholeheartedly acknowledge Dr. Jonathan Wirsirch (Project Mentor), Nicholas Blauch (Project TA), and Ishani Ganguly (Pod TA) for their valuable guidance and mentorship. We also acknowledge all the efforts, opportunities, and support provided by the entire Neuromatch Academy team.

### Brave-neurons (Team)

Ahmad Samara, Romeo Penheiro, Saksham Pruthi
