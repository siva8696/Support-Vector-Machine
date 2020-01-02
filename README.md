# Support-Vector-Machine
Support Vector Mahine is often called as SVM. It can do both classification and regression problems. In SVM, we will find the plane that best seperates the data with maximising the distance. 

![fig1](https://www.analyticsvidhya.com/wp-content/uploads/2015/10/SVM_21.png)


As you can see in fig1, we divided our data with the help of three hyperplanes i.e., A, B, C. You need to remember a thumb rule to identify the right hyper-plane: “Select the hyper-plane which segregates the two classes better”. In this scenario, hyper-plane “B” has excellently performed this job. Let's consider the above fig1 in different way as below

![fig2](https://www.analyticsvidhya.com/wp-content/uploads/2015/10/SVM_3.png)

Here, maximizing the distances between nearest data point (either class) and hyper-plane will help us to decide the right hyper-plane. This distance is called as Margin. Above, you can see that the margin for hyper-plane C is high as compared to both A and B. Hence, we name the right hyper-plane as C. Another lightning reason for selecting the hyper-plane with higher margin is robustness. If we select a hyper-plane having low margin then there is high chance of miss-classification.

![fig3](https://www.analyticsvidhya.com/wp-content/uploads/2015/10/SVM_10.png)

Let's consider the above fig, where the both classes are not linearly seperated. So how can draw a line to seperate the both the classes. 
In SVM, it is easy to have a linear hyper-plane between these two classes. But, another burning question which arises is, should we need to add this feature manually to have a hyper-plane. No, SVM has a technique called the kernel trick. These are functions which takes low dimensional input space and transform it to a higher dimensional space i.e. it converts not separable problem to separable problem, these functions are called kernels. It is mostly useful in non-linear separation problem. Simply put, it does some extremely complex data transformations, then find out the process to separate the data based on the labels or outputs you’ve defined.

Internally Sklearn, has the parameter called Kernal, where we can use different type of kernals so that it will take care of seperation of data in higher dimensions. We have a two type of SVM's one is called as "Hard Margin SVM" and another one is "Soft Margin SVM". Hard Margin only works well when we have a data linearly seperable. Where as in soft margin we will minimize the misclassified points from the actual hyperplane.

<h3>References :</h3>
https://medium.com/machine-learning-101/chapter-2-svm-support-vector-machine-theory-f0812effc72
https://www.analyticsvidhya.com/blog/2017/09/understaing-support-vector-machine-example-code/
