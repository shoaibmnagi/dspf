# Data Science Portfolio - Shoaib Mehmood


## Master's Thesis - Estimating House Prices through Machine Learning
 
 ![Distribution of Obsvs given Sale Price](/images/comb.png)
 
  For my Master's thesis at the University of Mannheim, I used machine learning algorithms to predict house prices in Germany and compare the results with the traditional hedonic pricing model. In the first part, I used four machine learning algorithms to estimate the house prices (Kernel Ridge Regression, Random Forests, Gradient Boosting Machines and Neural Networks). For each of these models, I tuned the hyperparamters using Random Search. 
  
  In the second part, I used Stacked Generalization to develop an ensemble meta-learner on the basis of my four machine learning algorithms. After compring the results, I concluded that the stacked ML model performs better than the traditional hedonic pricing model. 
  
  Code: [GitHub](https://github.com/shoaibmnagi/masters-thesis)


## Facial Mask Recognition using TensorFlow

![Training Loss & Accuracy](/images/accuracy.png)

  I take a dataset consisting of people wearing Covid-19 masks from Kaggle to train an algorithm to recognize masks in unseen pictures. I first convert the pictoral data into a CSV so I can use it to train my algorithm. Then, I use data augmentation to improve our generalization for our images. This is done to use our limited data and increase its diveristy. For example, data augmentation will randomly rotate, crop or adjust the pictures in your dataset to create less-than-perfect versions of it. This, later on, allows the algorithm to pick up newer observations that might not be 100% clear to the naked eye (for example, a person hanging upside down wearing a mask etc.).

 Then, I do some fine-tuning to adjust the weights of the head layer of our neural network. After this process is done, I finally compile and train my neural network algorithm using my traininig data (using ADAM optimizer). 
 
 I'm trying to integrate this algorithm with OpenCV, so I can use newer images from anywhere and let this algorithm figure out whether or not the person in the picture is wearing a mask. Once this is done, the project can be further exanded into one that can use video input to detect a fask mask.
 
 Code: [Kaggle](https://www.kaggle.com/shoaibmnagi/face-mask-detection)
