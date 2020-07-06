# Data Science Portfolio - Shoaib Mehmood


## Master's Thesis - Estimating House Prices through Machine Learning
 
 ![Distribution of Obsvs](https://github.com/shoaibmnagi/sm_dsportfolio/blob/master/chloropeth%20crope.png)
 
  For my Master's thesis at the University of Mannheim, I used machine learning algorithms to predict house prices in Germany and compare the results with the traditional hedonic pricing model. In the first part, I used four machine learning algorithms to estimate the house prices (Kernel Ridge Regression, Random Forests, Gradient Boosting Machines and Neural Networks). For each of these models, I tuned the hyperparamters using Random Search. 
  
  In the second part, I used Stacked Generalization to develop an ensemble meta-learner on the basis of my four machine learning algorithms. After compring the results, I concluded that the stacked ML model performs better than the traditional hedonic pricing model. 
  
  Code: [GitHub](https://github.com/shoaibmnagi/masters-thesis)


## Facial Mask Recognition using TensorFlow

![Training Loss & Accuracy](https://www.kaggleusercontent.com/kf/38196102/eyJhbGciOiJkaXIiLCJlbmMiOiJBMTI4Q0JDLUhTMjU2In0..pDCSfgJ3V1WElpXoRYDANw.W4EkI5TtoYf5qkioOF2sUqw84607RB8PpodAJoZAzlPORwcGMhlDYE845NZOw1oPdqWlL6nNWFPH28H8Q00SE9RKYf2mdE2YzXWUl8FBZSk25U3jU35X9sjH4vP3anMOMJSXR9Bcii47ankayDTGrJ1wMp2Iz_1OB0vTJIiODjl0AcTeCbUSo64SI7JNenafQet8fy4uiSqvRBNvkIroLU-m4ZF5JzhO1Uu4F6nu22N4af-R01j0Q5x5s2IQqTuof5ocpYhlt9RPZJ-JwfpTUBFr4ua7TyHU7PNqJ5aMi1liVomFaQBobvcjKKJGj7EuWaJSxzIzx2gPpm7HjjUwwTPbEglF-c2ddZvY235M57zc5aqsNoFUid-Z6OPSj3CFKmpNG3zVFTLKkjATKvSaf2C-VxtDfawBmBVKf1ew6rpUzO8dXNnLvt_5JUMe3fYXIi-IAmzilpGK3RoBbOY8LAUhXTMJekiAlNt8QRHmhcBJV2GkafUaj9pyFJAQ_D5AOOnxrV83hXhRniZHB8mvcaOGD8jYq-LTBmZuuI2qkiCUnmA4NtTAV3R3wM7tWwZ20wN1UV92x0sWc_yjarul8ieYo8TG__6dy3h0Ylvm9j8lnRe61niLmXIjQ61ebwKFGoWIwZewOczXIo4EV_ztsK3VShtx4vBU5jUHe6Ahttw.iIdcWslqk1ew8uW_JONaWw/__results___files/__results___9_3.PNG)

  I take a dataset consisting of people wearing Covid-19 masks from Kaggle to train an algorithm to recognize masks in unseen pictures. I first convert the pictoral data into a CSV so I can use it to train my algorithm. Then, I use data augmentation to improve our generalization for our images. This is done to use our limited data and increase its diveristy. For example, data augmentation will randomly rotate, crop or adjust the pictures in your dataset to create less-than-perfect versions of it. This, later on, allows the algorithm to pick up newer observations that might not be 100% clear to the naked eye (for example, a person hanging upside down wearing a mask etc.).

 Then, I do some fine-tuning to adjust the weights of the head layer of our neural network. After this process is done, I finally compile and train my neural network algorithm using my traininig data (using ADAM optimizer). 
 
 I'm trying to integrate this algorithm with OpenCV, so I can use newer images from anywhere and let this algorithm figure out whether or not the person in the picture is wearing a mask. Once this is done, the project can be further exanded into one that can use video input to detect a fask mask.
 
 Code: [Kaggle](https://www.kaggle.com/shoaibmnagi/face-mask-detection)
