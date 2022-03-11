# Topic Modeling State of the Union Addresses
Nate DiRenzo

## Abstract
The goal of this project was to identify the top 10 topics found in State of the Union addresses from 1790 - 2022. A subsequent goal was to assign probabilities for each of the 10 topics to each of the State of the Union addresses. After that, We clustered the addresses based on topic blend, and interpreted the clusters based on common topics and characteristics. Overall, the aim here was to see if there were distinct trends in the topics presidents discussed in State of the Union addresses or other characteristics. 
## Design
The design of this project was iterative. I started with a couple of different text preprocessing, vectorization, and topic modeling tools to see which performed best in terms of surfacing top 10 topics. I needed to tune the vectorizers with min_df and max_df, as well as custom stopwords, numerous times, and evaluated CountVectorizer and TF-IDF results in TruncatedSVD, Latent Dirichlet, and CorEx topic models. Once I selected my best-performing topic model, clustered the addresses based on topic probabilities, and interpreted the results for commonalities amongst the clusters.
## Data
The [dataset](https://www.kaggle.com/jyronw/us-state-of-the-union-addresses-1790-2019) contains all State of the Union addresses since 1790-2019. I manually added the 2022 State of the Union, because it was delivered last week. There are 220 addresses in total.

## Tools & Algorithms

*Data Wrangling*
- NLTK
- sklearn
- SpaCy
- pandas
- NumPy

*Topic Models and Clustering*
  
- Latent Dirichlet Allocation
- Truncated SVD
- CorEx
- KMeans Clustering

## Final Topic Model Results
  
Labor: program,job,economic,today,budget,help,goal,ahead,basic,worker
Manufacturing: crop,farmer,agriculture,farm,method,production,business,department commerce,type,interstate commerce
Government: constitution,outbreak,federal,supreme,amendment,service law,countryman,election,money order,total
Finance: cent,tariff,fiscal,expenditure,currency,treasury,end june,suggestion,postmaster,fiscal end
Social Issues: mexico,civil,protest,movement,immigration,slight,indian,citizenship,purely,lay senate
Foreign Policy: cuba,navy,army,japanese,consent,france,spain,rico,officer,panama
Science & Technology: research,technology,decade,achieve,challenge,environment,small business,cancer,leader,big
Law/Jurisprudence: court,hold,dangerous,perpetuity,commissioners district,department end,british north,fictitious,department end june,end june estimate
Education: school,student,education,college,university,math,street,teacher,medicare,tax credit
Infrastructure: interstate,railway,criminal,highway,commission appoint,colorado,consular service,naturalization,sign,bridge

## Interpretation

Cluster 1: 1913-1978, Labor, Manufacturing, Government, Science & Technology
Cluster 2: 1790-2022, Labor
Cluster 3: 1817-1909, Government, Manufacturing, Law
Cluster 4: 1845-1981, Labor
Cluster 5: 1827-1898, Government, Manufacturing, Finances
Cluster 6: 1843-1888, Labor
Cluster 7: 1790-1917, Government, Law
Cluster 8: 1825-1906, Manufacturing, Finance
Cluster 9: 1874-1956, Manufacturing, Labor
Cluster 10: 1841-1955, Labor


## Communication
See [Tableau](https://public.tableau.com/app/profile/nate.direnzo/viz/StateoftheUnionVisuals/Sheet4) visualizations.

See [PDF](https://github.com/NateDiR/sotu_nlp_project/blob/main/Topic%20Modeling%20the%20State%20of%20the%20Union%20Slides.pdf) for slides.