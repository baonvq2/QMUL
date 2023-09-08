Project topic: Predicting Rankings of Prop-tech Webpages on Google Organic Search Engine Result Pages

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
