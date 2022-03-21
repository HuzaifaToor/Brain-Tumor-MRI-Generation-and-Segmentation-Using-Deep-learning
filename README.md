# Brain Tumor MRI Generation and Segmentation Using Deep learning
 Brain Tumor has been affecting millions every year regardless of age, gender, or 
geographical differences. As it is highly complex to identify and categorize these 
tumors, researchers are keen to develop a mechanism that is not only able to 
intelligently identify the different parts of the tumor but also automatically 
segment it, making the work of a radiologist way easier. The scarcity of data in 
medical imaging along with its annotation hinders the usage of data-driven 
approaches such as deep learning algorithms. In this work, we proposed an 
approach based upon generative adversarial networks (GAN) for data 
augmentation. The approach consists of using two GAN models. The first model 
Deep Convolutional GAN (DCGAN) is trained on the BRAIN TUMOR 
SEGMENTATION (BraTS) dataset’s annotation/masks to generate new masks 
with the same underlining characteristics as the original masks. The second GAN 
model conditional GAN (CGAN) is trained on real data for the translation of the 
masks to its relative MRI. The CGAN model is used to translate the synthetic masks 
to MRI. These pairs of generated MRI and masks are used to augment the original 
dataset. The generated dataset was combined in different ratios to the original 
dataset. Segmentation network (SegNet) is trained on these different proportions 
of a combination of the dataset and to evaluate the trained model, a testing set was 
used from the original dataset with Jaccard coefficient as a metric. The results of 
the different combinations of the dataset were compared with that of the 
segmentation results when the only real dataset was used. An increase in the 
segmentation performance of the model was observed when it was trained on 
with a 25% addition of synthetic data to real data. The synthetic masks look 
visually closer to the real dataset masks; however, the synthetic MRIs do not look 
convincing which stills needs improvement
