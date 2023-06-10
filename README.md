# Graph-Datesets-of-Fraud-Detection
This repository is the compilation of fraud detection datasets, including multi-relation and single-relation graph datasets.
Alternative download source in Google Drive: (https://drive.google.com/drive/u/1/folders/1CQF0clK8Ngf65SdfTIVCEi3iF5azqd6g)
## Multi-relation Graph Datasets
Introduced by [Dou et al. in Enhancing Graph Neural Network-based Fraud Detectors against Camouflaged Fraudsters](https://dl.acm.org/doi/abs/10.1145/3340531.3411903)
* Amazon
The _Amazon_ includes reviews on musical instruments and takes users as nodes.
There are three different relations between nodes in Amazon: (1)__U-P-U__: users comment on at least one identical product; (2)__U-S-U__: users give at least one same rating within a week;  (3)__U-V-U__: users whose reviews rank in the top 5\% of in terms of TF-IDF similarity. 
* YelpChi
The _YelpChi_ contains reviews on hotels and restaurants in Chicago, which can be divided into spam and legit, and regards reviews as nodes. Meanwhile, the connection between nodes can also be defined as three types: (1)__R-U-R__: reviews posted by the common users; (2)__R-T-R__: reviews given the same star rating under the same item; (3)__R-S-R__: reviews issued by the same month under the identical item.
## Single-relation Graph Datasets

### Organic Fraud

- Elliptic 
The [Elliptic dataset](https://www.kaggle.com/datasets/ellipticco/elliptic-data-set) is a transaction graph collected from the Bitcoin blockchain. A node in the graph represents a transaction, an edge can be viewed as a flow of Bitcoins between one transaction and the other. Each node has 166 features and has been labeled as being created by a "licit", "illicit" or "unknown" entity.
- T-Finance
The [T-Finance dataset](https://proceedings.mlr.press/v162/tang22b.html) aims to ﬁnd the fraud accounts in transaction networks. The nodes are unique anonymized accounts related to registration days, logging activities and interaction frequency. The edges in the graph represent two accounts that have transaction records. Human experts annotate nodes as anomalies if they fall into categories like fraud, money laundering and online gambling.
- Disney
Flickr is an image hosting and sharing website. Similar to BlogCatalog, users can follow each other and form a social network. Node attributes of users are deﬁned by their speciﬁed tags that reﬂect their interests.
- Books
ACM is a citation network where each paper is regarded as a node on the network, and the links are the citation relations among diﬀerent papers. The attributes of each paper are generated from the paper abstract.
-Enron


### Injection Anomaly

Introduced by [Ding et al. in Interactive anomaly detection on attributed networks](https://dl.acm.org/doi/abs/10.1145/3289600.3290964)

- BlogCatalog
BlogCatalog is a blog sharing website. The bloggers in blogcatalog can follow each other forming a social network. Users are associated with a list of tags to describe themselves and their blogs, which are regarded as node attributes.
- Flickr
Flickr is an image hosting and sharing website. Similar to BlogCatalog, users can follow each other and form a social network. Node attributes of users are deﬁned by their speciﬁed tags that reﬂect their interests.
- ACM
ACM is a citation network where each paper is regarded as a node on the network, and the links are the citation relations among diﬀerent papers. The attributes of each paper are generated from the paper abstract.

# The statistics of the datasets

|  Dataset | #Nodes | Relation| #Edges | #Feat | #Con. | #Strct. | #Outliers | Outlier Ratio |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Amazon  | 11,944 |U-P-U <br> U-V-U <br> U-S-U <br> ALL|175,608 <br> 3,566,479 <br> 1,036,737 <br> 4,398,392| - | - | 821 | 6.87% |
| YelpChi  | 45,954 |R-U-R <br> R-T-R <br> R-S-R <br> ALL|49,315 <br> 573,616 <br> 3,402,743 <br> 3,846,979| - | - | 6,677 | 14.53% |
| Elliptic | 203,769 | - | 234,355 | 166 | - | - | 4,545 | 2.23% |
