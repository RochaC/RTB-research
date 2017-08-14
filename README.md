# RTB-research
RTB(Real-Time-Bidding) research walkthrough.
---- 
This is my research repo about the RTB, including code、data、paper and any other material I used. For now, all is about Demand-side-platform(DSP).

## Paper
---- 
### Bidding
- 

### CTR 
- [Practical Lessons from Predicting Clicks on Ads at Facebook](http://wnzhang.net/share/rtb-papers/fb-ad-ctr.pdf) by Xinran He et al. ADKDD 2014.
	  This paper formulate Normalized-Entropy as metrics and any other metrics explained. It also put forward the practice of GBDT+LR. (A method use GBDT(gradient boosting decision tree) to do feature transformation. 
	  
- [Predictive Model Performance: Offline and Online Evaluations](https://chbrown.github.io/kdd-2013-usb/kdd/p1294.pdf) by Jeonghee Yi, Ye Chen et al. KDD 2013.
	  This paper do the summary for now about the evaluation metrics of model performance including but not except sponsor search, RTB..et al. AUC is not good enough to evaluate model performance, RIG is not much good for model compare.

- [Logistic Regression in Rare Events Data](https://gking.harvard.edu/files/0s.pdf) by Gary King and Langche Zeng. Political Analysis 2001
	  This paper is about correction in LR model in rare events data namely the imbalanced dataset.

## dataset
---- 
- [iPinYou Real-Time Bidding Dataset for Computational Advertising Research](http://data.computational-advertising.org) 
	  This dataset is the PC traffic data about RTB. It’s about 3 seasons data. Detail about the benchmark and the data dictionary is in this paper [Real-Time Bidding Benchmarking with iPinYou Dataset](https://arxiv.org/pdf/1407.7073.pdf) by Dr.Zhang. 
