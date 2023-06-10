# Graph-Datesets-of-Fraud-Detection
This repository is the compilation of fraud detection datasets, including multi-relation and single-relation graph datasets.
## Multi-relation Graph Datasets
Introduced by [Dou et al. in Enhancing Graph Neural Network-based Fraud Detectors against Camouflaged Fraudsters](https://dl.acm.org/doi/abs/10.1145/3340531.3411903)
* Amazon
The _Amazon_ includes reviews on musical instruments and takes users as nodes.
There are three different relations between nodes in Amazon: (1)__U-P-U__: users comment on at least one identical product; (2)__U-S-U__: users give at least one same rating within a week;  (3)__U-V-U__: users whose reviews rank in the top 5\% of in terms of TF-IDF similarity. 
* YelpChi
The _YelpChi_ contains reviews on hotels and restaurants in Chicago, which can be divided into spam and legit, and regards reviews as nodes. Meanwhile, the connection between nodes can also be defined as three types: (1)__R-U-R__: reviews posted by the common users; (2)__R-T-R__: reviews given the same star rating under the same item; (3)__R-S-R__: reviews issued by the same month under the identical item.
## Single-relation Graph Datasets
### Injection Anomaly

Introduced by [Ding et al. in Interactive anomaly detection on attributed networks](https://dl.acm.org/doi/abs/10.1145/3289600.3290964)

- BlogCatalog
- Flickr
- ACM
