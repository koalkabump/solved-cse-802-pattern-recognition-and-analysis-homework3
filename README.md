Download Link: https://assignmentchef.com/product/solved-cse-802-pattern-recognition-and-analysis-homework3
<br>









<ol>

 <li>[15 points] Consider a set of <em>n </em>i.d. samples (one-dimensional training patterns), <em>D </em>= <em>{x</em><sub>1</sub>, <em>x</em><sub>2</sub>,… <em>x<sub>n</sub>}</em>, that are drawn from the following distribution (Rayleigh distribution):</li>

</ol>

<em>p</em>(<em>x|θ</em>)= 2<em>θ xe</em><em>−<sup>θ x</sup></em><sup>2</sup>,         <em>x ≥ </em>0,<em>θ&gt; </em>0.

<ul>

 <li><u>Derive </u>the maximum likelihood estimate (MLE) of <em>θ</em>, i.e., <em>θ</em><sub>b<em>mle</em></sub>.</li>

 <li>Consider a set of 1000 training patterns that can be accessed <a href="https://www.cse.msu.edu/~rossarun/courses/sp20/cse802/data/hw3_random_data_q1.txt"><strong>here</strong></a><a href="https://www.cse.msu.edu/~rossarun/courses/sp20/cse802/data/hw3_random_data_q1.txt">.</a> Plot the normalized histogram of the training patterns. In the same graph, plot the distribution, <em>p</em>(<em>x</em>), after estimating <em>θ</em><sub>b<em>mle </em></sub>from these training patterns.</li>

 <li>Using the same training patterns, determine the MLE estimates for the mean and variance of a Gaussian distribution. In this case, you can use the MLE formulae directly. Plot the resulting Gaussian distribution on the same graph as above.</li>

 <li>Comment on which of the two distributions better “fit” the training data.</li>

</ul>

<ol start="2">

 <li>[10 points] Let <em>x </em>have a uniform density</li>

</ol>

¨

1<em>/θ</em>,    0       <em>x θ</em>

<em>p</em>(<em>xθ</em>)<em>U</em>(0,<em>θ</em>)=                       <em>≤     ≤</em>

0,        otherwise.

<ul>

 <li>Suppose that <em>n </em>samples <em>D </em>= <em>{x</em><sub>1</sub>,… <em>x<sub>n</sub>} </em>are drawn independently according to <em>p</em>(<em>x|θ</em>). Show that the MLE for <em>θ </em>is max[<em>D</em>], i.e., the value of the maximum element in <em>D</em>.</li>

 <li>Suppose that <em>n </em>= 5 points are drawn from the distribution and the maximum value of which happens to be 0.6. Plot the likelihood <em>p</em>(<em>D|θ</em>) in the range 0 <em>≤ θ ≤ </em> Explain in words why you do not need to know the values of the other 4 points.</li>

</ul>

<ol start="3">

 <li>[15 points] Let <strong><em>x </em></strong>=(<em>x</em><sub>1</sub>,… <em>x<sub>d</sub></em>)<em><sup>t </sup></em>be a d-dimensional binary (0 or 1) vector with a multivariate Bernoulli distribution</li>

</ol>

<em>d</em>

Y <em>x</em><em>i − </em>1<em>−x</em><em>i </em>, <em>P</em>(<strong><em>xθ</em></strong>)= <em>θ</em><em>i </em>(1 <em>θ</em><em>i</em>)

<em>i</em>=1

where <strong><em>θ </em></strong>= (<em>θ</em><sub>1</sub>,…<em>θ<sub>d</sub></em>)<em><sup>t </sup></em>is an unknown parameter vector, <em>θ<sub>i </sub></em>being the probability that <em>x<sub>i </sub></em>= 1. Let <em>D </em>= <em>{<strong>x</strong></em><strong><sub>1</sub></strong>,… <strong><em>x<sub>n</sub></em></strong><em>} </em>be a set of <em>n </em>i.i.d. training samples. Show that the maximum likelihood estimate for <strong><em>θ </em></strong>is

<em>n</em>

1 X

<strong><em>θ</em></strong>b = <em>n      <strong>x<sub>k</sub></strong></em>.

<em>k</em>=1

(Hint: Consider deriving the MLE for a specific component, <em>θ<sub>i</sub></em>, of vector <strong><em>θ </em></strong>.)

<ol start="4">

 <li>[30 points] Consider a two-category (<em>ω</em><sub>1 </sub>and <em>ω</em><sub>2</sub>) classification problem with equal priors. Each feature is a two-dimensional vector <strong><em>x </em></strong>= (<em>x</em><sub>1</sub>, <em>x</em><sub>2</sub>)<em><sup>t</sup></em>. The <em>true </em>class-conditional densities are:</li>

</ol>

<em>p</em>(<strong><em>x</em></strong><em>|ω</em><sub>1</sub>) <em>∼ N</em>(<strong><em>µ</em><sub>1 </sub></strong>=[0,0]<em><sup>t</sup></em>,<em>Σ</em><sub>1 </sub>= <em>I</em>), <em>p</em>(<strong><em>x</em></strong><em>|ω</em><sub>2</sub>) <em>∼ N</em>(<strong><em>µ</em><sub>2 </sub></strong>=[5,5]<em><sup>t</sup></em>,<em>Σ</em><sub>2 </sub>= <em>I</em>).

Generate <em>n</em>=50 bivariate <em>random </em>training samples from each of the two densities.

<ul>

 <li>Write a program to find the values for the maximum likelihood estimates of <strong><em>µ</em><sub>1</sub></strong>, <strong><em>µ</em><sub>2</sub></strong>, <em>Σ</em><sub>1</sub>, and <em>Σ</em><sub>2 </sub>using these training samples (see page 89, use equations (18) and (19)).</li>

 <li>Compute the Bayes decision boundary using the <em>estimated </em>parameters and plot it along with the training samples. What is the empirical error rate on the training samples?</li>

 <li>Compute the Bayes decision boundary using the <em>true </em>parameters and plot it on the same graph. What is the empirical error rate on the training samples?</li>

 <li>Repeat (a) – (c) after generating <em>n</em>=500 and <em>n</em>=50,000 random training samples from each of the two densities. How do the estimated parameters and the empirical error rate change in (a) and (b) when the number of representative training samples increases?</li>

</ul>

<ol start="5">

 <li>[20 points] The <a href="https://www.cse.msu.edu/~rossarun/courses/sp20/cse802/data/iris_data.txt"><strong>iris (flower) dataset</strong></a> consists of 150 4-dimensional patterns (i.e., feature vectors) belonging to three classes (setosa=1, versicolor=2, and virginica=3). There are 50 patterns per class. The 4 features correspond to sepal length in cm (<em>x</em><sub>1</sub>), sepal width in cm (<em>x</em><sub>2</sub>), petal length in cm (<em>x</em><sub>3</sub>), and petal width in cm (<em>x</em><sub>4</sub>). Note that the class labels are indicated at the end of every pattern.</li>

</ol>

Assume that each class can be modeled by a multivariate Gaussian density, i.e., <em>p</em>(<strong><em>x</em></strong><em>|ω<sub>i</sub></em>) <em>∼ </em>N(<strong><em>µ</em></strong><em><sub>i</sub></em>, <strong><em>Σ</em></strong><em><sub>i</sub></em>), <em>i </em>= 1,2,3. Write a program to design a Bayes classifier and test it by following the steps below:

<ul>

 <li>Train the classifier: Using the first 25 patterns of each class (training data), compute <strong><em>µ</em></strong><em><sub>i </sub></em>and <strong><em>Σ</em></strong><em><sub>i</sub></em>, <em>i </em>= 1,2,3. <strong>Report </strong>these values.</li>

 <li>Design the Bayes classifier: Assuming that the three classes are equally probable and a 0-1 loss function, write a program that inputs a 4-dimensional pattern <strong><em>x </em></strong>and assigns it to one of the three classes based on the maximum posterior rule, i.e., assign <strong><em>x </em></strong>to <em>ω<sub>j </sub></em>if,</li>

</ul>

<em>j </em>= arg max <em>{P</em>(<em>ω<sub>i</sub>|<strong>x</strong></em>)<em>}</em>.

<em>i</em>=1,2,3

<ul>

 <li>Test the classifier: Classify the remaining 25 patterns of each class (test data) using the Bayes classifier constructed above and report the confusion matrix for this three-class problem. What is the empirical error rate on the test set?</li>

</ul>

<ol start="6">

 <li>[20 points] The <a href="https://www.cse.msu.edu/~rossarun/courses/sp20/cse802/data/imox_data.txt"><strong>IMOX</strong></a> dataset consists of 192 8-dimensional patterns pertaining to four classes (digital characters ‘I’, ‘M’, ‘O’ and ‘X’). There are 48 patterns per class. The 8 features correspond to the distance of a character to the (a) upper left boundary, (b) lower right boundary, (c) upper right boundary, (d) lower left boundary, (e) middle left boundary, (f) middle right boundary, (g) middle upper boundary, and (h) middle lower boundary. Note that the class labels (1, 2, 3 or 4) are indicated at the end of every pattern.

  <ul>

   <li>Write a program to project these 8-dimensional points onto a two dimensional plane using PCA (the top 2 eigenvectors). Report the two projection vectors estimated by the technique. Plot the entire dataset in two dimensions using these projection vectors. Use different markers to distinguish the patterns belonging to different classes.</li>

   <li>Write a program to project these 8-dimensional points onto a two dimensional plane using MDA (the top 2 eigenvectors). Report the two projection vectors estimated by the technique. Plot the entire dataset in two dimensions using these projection vectors. Use different markers to distinguish the patterns belonging to different classes.</li>

   <li>Discuss the differences between the PCA and MDA projection vectors.</li>

  </ul></li>

 <li>[20 points] Assume that the features in the 4-class 8-dimensional <a href="https://www.cse.msu.edu/~rossarun/courses/sp19/cse802/data/imox_data.txt"><strong>IMOX</strong></a> dataset described above are statistically independent. Further, assume that each feature for each of the four classes is normally distributed, i.e., <em>p </em><em>| </em>, where <em>i </em>= 1…8 and <em>j </em>= 1…4.

  <ul>

   <li>Report the MLE estimates of the mean and variance of each feature for each class, i.e., compute <em>µ</em>Ó<em><sub>ij </sub></em>and <em>σ</em><sub>Ó</sub><sup>2</sup><em><sub>ij</sub></em>, for <em>i </em>= 1…8 and <em>j </em>= 1…4.</li>

   <li>Assuming a 0-1 loss function and equal priors (and statistically independent features having a Gaussian form), design a Bayesian classifier that inputs an 8-dimensional pattern and assigns it to one of the four classes.</li>

   <li>Train this classifier using the first 24 patterns of each class (so, a total of 96 training patterns). Report the confusion matrix and the empirical error rate of this classifier on the remaining 24 patterns of each class (so, a total of 96 test patterns).</li>

  </ul></li>

 <li>[20 points] Consider a dataset in which every pattern is represented by a set of 15 features. The goal is to identify a subset of <u>5 features or less </u>that gives the best performance on this dataset. How many feature subsets would each of the following feature selection algorithms consider before identifying a solution (i.e., the number of times the criterion function, <em>J</em>(.), will be invoked)?

  <ul>

   <li>SFS;</li>

   <li>Plus-<em>l</em>-take-away-<em>r </em>with (<em>l</em>, <em>r</em>)=(5,3);</li>

   <li>SBS;</li>

   <li>Exhaustive Search</li>

  </ul></li>

</ol>