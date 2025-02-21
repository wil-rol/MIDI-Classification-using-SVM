# MIDI-Classification-using-SVM
 This project focused on classifying MIDI files from six composers—Albeniz, Anglebert, Dowland, Pachelbel, Palestrina, and Telemann—using Support Vector Machines (SVM).

 # Dataset
 Each composer file contained roughly 60 files, with a total of 378 files. After removing 2 files that are duplicates, the dataset contains 376 files before separating into training and test set. These composers were chosen 
 because they had a similar number of MIDI files, which would make the distribution of composers more balanced across the dataset. Imbalances in the dataset can strongly affect the SVM model training.

 # Methods
 Supervised machine algorithms known as SVM are used to classify MIDI files based on features extracted from the data. They work by finding the optimal hyperplane that separates data points of different classes into higher 
 dimensional space, which is commonly referred to as the kernel trick. A hyperplane is a decision boundary used to separate two different classes. The goal is to maximize the margin, or the distance between the hyperplane 
 and the nearest support vectors. SVMs are commonly used for classification and regression tasks because they are resistant to noisy data, while also working well with linear and non-linear data. Four SVM models were 
 created to test how different kernel types would affect classification results. The four kernel functions used are linear, polynomial, radial basis function (RBF), and sigmoid. These different SVM models will be used to 
 fit or train the model using provided training data and corresponding target labels. During this process, the model learns patterns and relationships in the data that are used to make predictions about data outside of the
 training set.

 # Results
 The RBF model performed the best based on the evaluation metrics. It achieved the highest test accuracy of 0.92 and the highest average cross-validation accuracy on the training set
 of 0.7161. This model also had a total of 3 misclassified data points, which is the least of all the SVM models. The linear model performs relatively well and is closely comparable to the RBF model.
 The linear model achieves a test accuracy of 0.91 and the average cross-validation accuracy on the training set is 0.7132. This model has the second least misclassifications with a total of 4.
 The polynomial and sigmoid models exhibited the most variance when tuning hyperparameters and were clearly outperformed by the RBF and linear models.
 
![features_df](https://github.com/user-attachments/assets/fb8ceffc-4f90-427c-9ca3-6ac535caf962)

![rbf_conf_mat](https://github.com/user-attachments/assets/9f96cfa9-3bed-484d-b229-5f03c0e0ebbd)

![linear_conf_mat](https://github.com/user-attachments/assets/94e723b3-f426-4c6f-811b-29deade63bbe)

![poly_conf_mat](https://github.com/user-attachments/assets/4997506c-1ca2-4253-b792-8613ccbba553)

![sig_conf_mat](https://github.com/user-attachments/assets/1ee5d094-3ec5-4dd8-8e60-a12ab7225a50)

![results_df](https://github.com/user-attachments/assets/5a32e000-066d-4513-bda5-497fc0d211c6)
