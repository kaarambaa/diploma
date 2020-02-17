## Abstract (удалить само слово Abstract перед отправкой)

## Introduction
### Background
The e-commerce market is showing rapid growth during past decade and this growth is going to continue in the nearest future. However, customer behavior has changed significally and established ways of doing busiess are getting less effective every year. Standart "best" practices were aimed at interacting with segments of customers while now, techologies can allow business to concentrate on exact customer and to interact with him. According to the latest researches from leading world sources, personalization in e-commerce has become one of the strongest influencers on customer experience. Well-tuned personal recommendations can provide high level of customer satisfaction and, consequently, stable increase of revenue, generated on this website. Furthermore, according to Netflix statistics, if user doesn't choose what he/she want to watch in first three minutes of search – he/she will lose interest and leave the website (or the smartphone app) without any actions, within the realities of an e-commerce it means that user will simply leave online shop without any purchase. That is why it is essential to understand clearly how to provide personal recommendation and which tool to use.
The theoretical objests of this paper will be recomendational systems and variaties of their applicability in e-commerce companies.  
### Problem statement
As it has already been metioned, personalization has become an important part of online business. Significant increase in data-driven technologies in the last decade led to appearance multiplicity of tools which could help businesses to provide direct recomendations. However, many companies still do not use solutions which can provide the highest efficiency due to the big variaty of them and due to the complexity of their selecting, development and deployment.  
Due to large amount of data, which every e-commerce company can collect daily, it is becomming extremely tough to find insides in this informational manualy. That is why the necessity in machine learning models, which can perform difficult calculations and predictions in a short time, is increasing rapidly. Certainly it is possible to create personal recomedations without big data in general and machine learning in particular. It is acceptable to use such semi-manual tools when goods, which company sell, are specific and do not have many substitutes. Nevertheless, when the list of subsidaries expands, benifits from such tools decreases drammaticaly. It will take too much time and 
consequently money to create links between hundreds of similar or complementive products in a manual way, while the accuracy of such system would be much lower than it could be with data-driven model. So, it is essentil to company's management to select the right recomendation systmen to maximize their direct recomendations efficiency from the very beggining of doing business.  
This paper is aimed to help business owners, especially that ones, who has just started their business and who has lack of technical knowledge to select recomedational system which will be most suitable for the particular business.
To achive the goal of the research it is necessary to implement the following tasks:
1. To make an introduction into machine learning basics to provide basic knowledge of technologies which are being used in the personal recomendations creating process.
2. To collect data for machine learning models training
3. To develop demonstation versions of recomendation systems, which will be able to demonstrate their applicability in different business circumstances.
4. Conduct a comparsion of selected recomendation systems using accuracy, precision and recall metrics.
5. Based on results, make a list of recommendations for companies' management on choosing the right recomendation system.  
### Professional significance.
The research involves the creation of recommendations created on the basis of assesing several recomendation algoritms that companies' management can use in the selecting and deployment process of the recomendation system in their business. Created models cannot be used as they are in the production
and are for demonstration purposes only. However, if any of them is re-trained on the real business data - it will be able to provide simple recomendations with moderate accuracy.  
### Delimitations of the study
Due to the limited number of training datasets, which can be found in the free access, all models, which will be developed during this research, will be trained on the MovieLens dataset. It is a public dataset, which is provided by the University of Minnesota. It consist of 100000 raitings applied to 9000 movies by 600 users and perfectly fits academic purposes. However, owing to the specificity of the data, these models can not be used in the business task without re-training on the data, connected to the particular market.
## Definitions of key terms
First of all, it is vital to identify the definition of the customer expierence as the essential purpose of recomendational system implementation into the business. There were numerous of different definitions of customer expiernce in literature, while the most exhaustive one was given by K. Lemon (2016): "customer experience is a multidimensional construct focusing on a customer’s cognitive, emotional, behavioral, sensorial, and socialresponses to afirm’s offerings during the customer’s entirepurchase journey".
The second term, which shuld be undercovered is "Machine Learning". Machine learning is an application of artificial intelligence that provides systems the ability to automatically learn and improve from experience without being explicitly programmed. Machine learning focuses on the development of computer programs that can access data and use it learn for themselves.
The third basic concept of this paper is "recommendation systems". This generalized concept includes a number of machine learning models which provides recommendations to customers  based on their preferences and other data, connected with pucrchaeses and purchuased goods.

## Main body
### Lirearure review
The following paper will describe recomender systems as a strong influencer on customer loyality. 

According to [1], the recommender systems can be defined as a cognitive system, which collects data from the users' activities logs and provides a set of recommended items. The first recommender system which was able to generate automated predictions was the GroupLens system [Resnick et al. 1994; Konstan et al. 1997]. It provided personalized recommendations on the huge library of scientific papers. The recommendations for each individual were generaterd by identifying clusters of similar subscribers and suggesting them articles that other members of the group found useful.  
There are two  core approaches  for creating and training  recommender  systems: content-based filtering,  which creates customers and items profiles based on historical data and recommends items with similar profiles (Lang, 1995; Melville et al., 2002), and collaborative  filtering, which predicts users’ behaviors based on similarity of users' prefferences (Bell and Koren, 2007).

   
Nowadays there are two core types of recommeder systems:
- Content-based systems [2] which use the historical data of user's purchases and recommend items, which are similar to those ones which user has already purchased.
- Collaborative filtering systems [3] which devides customers into clusters according to their preferences and after that recomend items, which relate to the field of interests of each cluster. [1088 words]



1. Resnick, P., & Varian, H. R. (1997). Recommender systems. Communications of
the ACM, 40(3), 56-58.
2.   Tong Zhang, Vijay S. Iyengar Recommender Systems Using Linear Classifiers // Journal of Machine Learning Research . - 2002. - №2. - С. 313 - 334.
3. Gabor Takacs, Istvan Pilaszy, Bottyan Nemeth, Domonkos Tikk Scalable Collaborative Filtering Approachesfor Large Recommender Systems // Journal of Machine Learning Research . - 2009. - №10. - С. 623 - 656.
4. Xuan  Bi,  Annie  Qu,  Junhui  Wang,  and  Xiaotong  Shen.   A  group-specific  recommendersystem.Journal of the American Statistical Association, 112(519):1344–1353, 2017.
5. Robert M Bell and Yehuda Koren. Scalable collaborative filtering with jointly derived neigh-borhood interpolation weights.  In7th  IEEE  International  Conference  on  Data  Mining(ICDM 2007), pages 43–52. IEEE, 2007
6. Ken Lang. Newsweeder: Learning to filter netnews. In Proceedings of the 12th International Conference on Machine Learning, pages 331–339, 1995.
7. Prem Melville, Raymond J Mooney, and Ramadass Nagarajan.  Content-boosted collabo-rative filtering for improved recommendations.AAAI/IAAI, 23:187–192, 2002.
