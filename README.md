# UnifiedAttri2vec-
Unified Link Prediction: Leveraging Multi-Algorithm Embeddings and Attri2Vec:
This repository provides the official implementation of the UnifiedAttri2Vec-LSTM framework for link prediction in static attributed networks. The model integrates attribute-based and structural node representations through hierarchical fusion and models higher-order feature dependencies using an LSTM classifier.
**Installation**
git clone https://github.com/Fatima-Ziya/UnifiedAttri2veccode
cd UnifiedAttri2Vec-LSTM
pip install -r requirements.txt
**NOTE: *At this stage, our manuscript is under review in Chaos. The implementation code is currently maintained in a private repository to ensure confidentiality during the peer-review process. Upon receiving the final editorial decision, we will release the complete source code to a public repository to support transparency, reproducibility, and further research.*
**Dataset Preparation**Example
Datasets used in the paper:
Cora
CiteSeer
PubMed
Facebook
Amazon
US Air Transportation Network
Western States Power Grid
C. elegans Neural Network
**python src/dataset_loader.py --dataset cora**
**Data Preprocessing Pipeline**
1. Graph Representation
Load node list and edge list.
Construct undirected graph G=(V,E).
Remove self-loops and duplicate edges.
2. Feature Matrix Preparation
3. Train/Test Split
4. Attributed Embedding Generation
5. Structural Embedding Generation
6. Hierarchical Fusion
7. Edge Embedding Generation
8. LSTM Input
9. Model Training
    **python train.py --dataset cora**

UnifiedAttri2Vec-LSTM/
│
├── data/
│   ├── cora/
│   ├── citeseer/
│   ├── pubmed/
│   └── processed/
│
├── preprocessing/
│   └── preprocess.py
│
├── models/
│   ├── attri2vec.py
│   ├── fusion.py
│   └── lstm_classifier.py
│
├── train.py
├── evaluate.py
├── utils.py
└── README.md



