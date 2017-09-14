# RTB-research

## RTB\(Real-Time-Bidding\) research walk through.  

This is my material repo about the Computional Advertising. That's about the resource i read, some notes and memo.   

Welcome to make friends in this industry. 

# Book

- **[Display Advertising with Real-Time Bidding (RTB) and Behavioural Targeting](https://arxiv.org/abs/1610.03013) by Jun Wang, Weinan Zhang and Shuai Yuan. ArXiv 2016.**  

  A very detail introduction book about RTB industry and technic detail with many paper reference.

- **Computational Advertising by Peng Liu, Chao Wang. 2015**  

  A good introduction book from almost all perspectives to talking about digital advertising. Copyright reserve. So no link..

## Paper

### Bidding

- **[Optimal Real-Time Bidding for Display Advertising](http://discovery.ucl.ac.uk/1496878/1/weinan-zhang-phd-2016.pdf) by Weinan Zhang. PhD Thesis 2016.**  

  Very excellent work about bid optimalization.  Detail research in the future.

- **[Optimal Real-Time Bidding for Display Advertising](http://wnzhang.net/share/rtb-papers/optimal-rtb.pdf) by Weinan Zhang, Shuai Yuan, Jun Wang. KDD 2014.**   
  This paper give theory foundation of optimal bidding algorithm which take budget and win rate into consideration. It prove to be an nonlinear bidding. The experiment result is better than the linear one. 

- **[Bid Optimizing and Inventory Scoring in Targeted Online Advertising](http://wnzhang.net/share/rtb-papers/lin-bid.pdf) by Claudia Perlich et al. KDD 2012.** [PPT is here](https://www.samsi.info/wp-content/uploads/2016/03/perlich_august2012.pdf)

  This paper put forward the theory of a bidding algorithm now known as linear bidding. Use CTR as user experience feedback to adjust the system. But the linear bidding doesn’t take budget into consideration and will spent the money quickly if there’s no pace control. 

  ​

### CTR

* **[Simple and Scalable Response Prediction for Display Advertising](http://wnzhang.net/share/rtb-papers/ctr-chapelle.pdf) by Olivier Chapelle Criteo, Eren Manavoglu, Romer Rosales. ACM TIST 2014.**

  Very specific CTR modeling process.

* **[Practical Lessons from Predicting Clicks on Ads at Facebook](http://wnzhang.net/share/rtb-papers/fb-ad-ctr.pdf) by Xinran He et al. ADKDD 2014.**    

  This paper formulate Normalized-Entropy as metrics and any other metrics explained. It also put forward the practice of GBDT+LR. \(A method use GBDT\(gradient boosting decision tree\) to do feature transformation.


* **[Ad Click Prediction: a View from the Trenches](https://www.eecs.tufts.edu/%7Edsculley/papers/ad-click-prediction.pdf) by H. Brendan McMahan. KDD 2013.**

  This paper have a lot of pratical skills and industry experience about CTR, including sparsification, feature enginering, validation and final calibration. It also put forward how to estimate the unconfidence pCTR. The calibration is about possion regression or isotonic regression.(Need further check.)

* **[Predictive Model Performance: Offline and Online Evaluations](https://chbrown.github.io/kdd-2013-usb/kdd/p1294.pdf) by Jeonghee Yi, Ye Chen et al. KDD 2013.**    

  This paper do the summary for now about the evaluation metrics of model performance including but not except sponsor search, RTB..et al. AUC is not good enough to evaluate model performance, RIG is not much good for model compare.

- **[Estimating Conversion Rate in Display Advertising from Past Performance Data](http://wnzhang.net/share/rtb-papers/cvr-est.pdf) by Kuang-chih Lee et al. KDD 2012.**

  This paper explain a method like clustering the similar user whom has conversion to deal with the sparsity data. It also include some pratical technic skills like imbalanced dataset processing, result calibration. Experiment prove that the skewness would not affect the model performance but the probability scores it output and it still need calibrate.

###  

### Other Technique Tricks

- **Steffen Rendle (2010): *[Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf)*, in Proceedings of the 10th IEEE International Conference on Data Mining (ICDM 2010), Sydney, Australia.**

  Factorization machine. Widely used in Information Retrieve field. It extend LR, take 2nd  cross-feature into consideration. The idea is simple. But very useful.

  ​

- **[Feature Hashing for Large Scale Multitask Learning](http://www.machinelearning.org/archive/icml2009/papers/407.pdf), by Kilian Weinberger et al.  2010**

  This paper show great details about feature hash, including mathematic prove, application in spam email filter. NLP problem. It could also apply when there's need to reduce RAM. But google shows that, hash trick may induce great bias when there's great collision.

  ​

- **[Logistic Regression in Rare Events Data](https://gking.harvard.edu/files/0s.pdf) by Gary King and Langche Zeng. Political Analysis 2001**  

  This paper is about correction in LR model in rare events data, the imbalanced dataset. Two correction methods, afterward correction and weight correction.

## Dataset

---

* **[iPinYou Real-Time Bidding Dataset for Computational Advertising Research](http://data.computational-advertising.org)**   

  This dataset is the PC traffic data about RTB. It’s about 3 seasons data. Detail about the benchmark and the data dictionary is in this paper [Real-Time Bidding Benchmarking with iPinYou Dataset](https://arxiv.org/pdf/1407.7073.pdf) by Dr.Zhang.



