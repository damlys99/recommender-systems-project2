# Project 2: Neural Networks Recommender

That project is a simple recommender based on data from hotels. Created for Recommender Systems Class conducted by [@PiotrZiolo]( https://github.com/PiotrZiolo )

## Requirements:

1. Create (and activate) a new environment with Python 3.8 with conda.

    * Linux or Mac:
        ```console
        conda create --name recommender python=3.8
        source activate recommender
        ```
    * Windows:
    
        ```console
        conda create --name recommender python=3.8 
        activate recommender
        ```

2. Install jupyter notebook
    
    ```console
    pip install notebook 
    ```
    
3. Install all needed packages

    ```console
    pip install numpy pandas matplotlib seaborn ipython sklearn hyperopt
    ```

4. Start Jupyter Notebook
    * project\_1\_data_preparation.ipynb contains the process of preprocessing data
    * project\_2\_recommender\_and\_evaluation contains recommender

## Algorithms used
    * NeuMFModel
    * AdamW Optimizer

|    | Recommender         | HR@1      | HR@3      | HR@5      | HR@10     | NDCG@1    | NDCG@3    | NDCG@5    | NDCG@10  |
|----|---------------------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|----------|
| 0  | NNRecommender       | 0.045146  | 0.121521  | 0.164291  | 0.227427  | 0.045146  | 0.088711  | 0.106581  | 0.126703 |
| 1  | AmazonRecommender   | 0.044128  | 0.118805  | 0.160557  | 0.223693  | 0.044128  | 0.086755  | 0.104216  | 0.124468 |
| 2  | NetflixRecommender  | 0.045146  | 0.121860  | 0.164291  | 0.229124  | 0.045146  | 0.088881  | 0.106604  | 0.127288 |