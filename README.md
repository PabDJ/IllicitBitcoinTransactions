# IllicitBitcoinTransactions
Generation and classification of illicit Bitcoin transactions through Artificial Intelligence

This repository contains the code involved in the paper [Generation and Classification of Illicit Bitcoin Transactions](https://link.springer.com/chapter/10.1007/978-3-031-21333-5_108)

To support this research please consider citing:

``de Juan Fidalgo, P., Cámara, C., Peris-Lopez, P. (2023). Generation and Classification of Illicit Bitcoin Transactions. In: Bravo, J., Ochoa, S., Favela, J. (eds) Proceedings of the International Conference on Ubiquitous Computing & Ambient Intelligence (UCAmI 2022). UCAmI 2022. Lecture Notes in Networks and Systems, vol 594. Springer, Cham. https://doi.org/10.1007/978-3-031-21333-5_108``

## Abstract
> Financial fraud is an everyday problem that banking institutions have to face. With the disruption of Bitcoin as a new model which relies on decentralization and anonymity, attackers have taken advantage of this monetary system that allows them to obtain funds from illegal activities such as ransomware payments or terrorist organizations financing. At the same time, Law Enforcement Agencies use the availability of Blockchain data in order to detect suspicious transactions. The problem is that this task is usually performed by artificial intelligence and the current situation shows us a scarcity of high quality data sets. Algorithms do not have enough samples to learn the different patters that are hidden behind illicit Bitcoin transactions. This thesis tries to overcome this problem with significant contributions. We have increased in nearly 25,000 illicit transactions the Elliptic Data Set, which is the largest labelled transaction data set publicly available in any cryptocurrency. The former data set only contained 4,545 illicit transactions, resulting in a class imbalance of 9.8:90.2 illicit/licit ratio. Our work has changed that to a 41.2:58.8 illicit/licit ratio. In order to show that class imbalance can also be beaten with artificial work, we have studied the use of generative adversarial networks (GAN) for creating synthetic samples. The last part of this thesis was dedicated to the study of long short- term memory networks (LSTM) for the binary classification problem of detecting illicit Bitcoin transactions. The current state of the art is mainly focused on machine learning algorithms and we have showed that deep learning is getting promising results and can be an alternative solution for the future.

## Files
- suspicious_addresses.txt: 13,500 Bitcoin addresses linked to ransomware campaigns and Ponzi schemes.
- get_tx_from_addresses.ipynb: script for collecting transactions from the Bitcoin addresses through Blockstream API.
- tx_from_suspicious_addresses.csv: file that contains near 25,000 illicit transactions from the suspicious Bitcoin addresses
- TGAN/Elliptic_TGAN.ipynb: Jupyter notebook file that allow us to generate artificial Bitcoin transactions from the sample illicit.csv, which is the file that contains the illicit transactions from Elliptic Data Set.
- Machine_learning_RandomForest_LogisticRegression.ipynb: Jupyter notebook with Random Forest and Logistic Regression code for binary classification.
- LSTM.ipynb: Jupyter notebook with Long short-term memory network code for binary classification.

## Data Sets
We have increased in nearly 25,000 illicit transactions the Elliptic Data Set, which is the largest labelled transaction data set publicly available in any cryptocurrency. The former data set only contained 4,545 illicit transactions, resulting in a class imbalance of 9.8:90.2 illicit/licit ratio. Our work has changed that to a 41.2:58.8 illicit/licit ratio. 

Data set at Kaggle: [Augmented Elliptic Data Set](https://www.kaggle.com/datasets/pablodejuanfidalgo/augmented-elliptic-data-set)

Original data set: [Elliptic Data Set](https://www.kaggle.com/datasets/ellipticco/elliptic-data-set)

Synthetic generation can be found at TGAN/Elliptic_TGAN.ipynb file.
