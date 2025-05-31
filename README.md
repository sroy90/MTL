First, download the dataset from the following Kaggle link and unzip it — you will find both the required .txt files (citation-network2.txt and AMiner-Author.txt) inside: https://www.kaggle.com/datasets/kmader/aminer-academic-citation-dataset?resource=download.

To execute the model successfully, please follow these steps:

Required Files
Ensure the following three files are placed in the working directory before running the notebook:

citation-network2.txt

AMiner-Author.txt

fairness_values.pkl

Execution Steps

first
Run Data Preprocessing
Open data_preprocessing.ipynb using Jupyter Notebook, VS Code, or Google Colab.

Execute each code block sequentially from top to bottom without skipping any cells.

This will generate a file named:
paper_author_vectors.pkl

This step prepares the input vectors for the model including:

One-hot encoding for each paper ID

Multi-hot encoding for associated authors

Fairness score per paper

second
Run the Model
Open MTL_model.ipynb.

Run all the cells in order.

This notebook uses the paper_author_vectors.pkl file from the previous step and runs the Multi-Task Learning (MTL) model.
