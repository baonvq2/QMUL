**Project topic: Predicting Rankings of Prop-tech Webpages on Google Organic Search Engine Result Pages**

#Ranking #Learning-To-Rank #prop-tech #GoogleSEO

The paper focuses on addressing ranking prediction problems by applying Learning-To-Rank (LTR) methods, specifically pointwise, pairwise, and listwise approaches. LTR has demonstrated its usefulness and effectiveness in
tackling such problems. The study aims to implement these prediction methods in a real-world ranking context and showcases their performance comparison across the validation dataset. Five models, including pointwise,
RankNet (pairwise), LambdaRank (pairwise), LambdaMART (pairwise), and ListNet (listwise), are tested to determine the best-performing approach. While the pointwise, RankNet, and listwise models are constructed
using Neural Network, the other two methods utilize available built-in models from the LightGBM and XGBoost libraries. The experimentation is conducted, using a carefully collected dataset from the UK prop-tech industry. Notably,
the dataset and the data collection process stand out as the project highlights, offering valuable resources and frameworks for future related studies, both as reusable assets and as insightful directions for further research. The results
reveal that ListNet has outperformed the other models in predicting actual rankings, achieving an average Normalized Discounted Cumulative Gain (NDCG) score of over 0.95. This demonstrates the effectiveness of the listwise approach
in capturing the relationships among URLs within a query and producing highly accurate predictions. Additionally, the subsequent analysis highlights the significant contributions of factors, such as page experience, embedded links, and
certain HTML content, like total images or keyword presence in titles and URLs, to the model's prediction performance. These insights provide valuable guidance for online marketers seeking to optimize their webpage rankings and
overall search engine visibility. Moreover, the research offers practical implications and suggestions for related future works, paving the way for further advancements in ranking prediction techniques and SEO strategies. The study's
comprehensive evaluation of different LTR methods and its emphasis on real-world applicability make it a valuable contribution to the field of ranking prediction.

**Result**:

The boxplot of NDCG performance among the models in Figure 1 provides valuable insights into how each model's evaluation metric varies across search queries and across different test sets, created with random seed of 1, 5 and 7.
While the pointwise, LambdaRank, and LambdaMART models exhibit commendable performances, the ListNet model stands out as the better choice for the prediction task. Not only does it produce slightly higher NDCG scores, but it
also demonstrates lower variance across all queries and the selected test datasets, indicating its robust performance. If purely based on the NDCG, with the performance averaging at over 0.95, ListNet, a listwise method, proves to
be the most suitable and effective choice for this study. Its performance in accurately predicting rankings further reinforces its value and relevance in the research context.

![image](https://github.com/baonvq2/QMUL/assets/110440601/6c513799-56ca-4d93-ad82-44f64a828a20)












In the supporting materials, there are total 6 files, including:
	- 4 Jupyter notebooks (.ipynb): 
		+ Data collection (Data Collection-Final.ipynb): a thorough data collection process, including extracting general data, Page experience metrics and other html/content-related factors
		+ Pagerank calculation (PageRank-Final.ipynb): using NetworkX and collected links
		+ Model construction and learning (Model Build-Final.ipynb): building models, tuning and generate performance on selected test data; insights into feature importance
		+ Model validation and selection (Model Validation-Final.ipynb): validate model on different test data (seeds) and visualize the performances
	- 2 excel files (.xlsx):
		+ Selected keywords (Final_kw.xlsx): final list of chosen search keywords, used for 'Data collection'
		+ Final data (processed_data.xlsx): collected data after implementing 'Data collection' and 'Pagerank calculation', used in 'Model construction and learning' and 'Model validation and selection'

The process of using the file should be like this:
	- Stage 1: 'Data collection' & 'Pagerank calculation'
	- Stage 2: 'Model construction and learning'
	- Stage 3: 'Model validation and selection'

Below is modules/libraries that need to be installed for running the notebooks:
	- basic packages: numpy, pandas, os, IPython, time, datetime, matplotlib, seaborn, operator, statistics
	- torch
	- torchvision
	- pytorchltr
	- lightgbm
	- xgboost (version 2.0.0)
	- sklearn
	- skopt, optuna
	- captum
	- shap
	- modules for data collection: requests, json, urllib, requests_html, undetected_chromedriver, selenium, bs4, whois, warnings
	- networkx
