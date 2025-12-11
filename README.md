# AI-Generated-Text-Detection-Using-Comparative-Embedding-and-Classification-Methods
 **ELEC 877 Research Project:** 
Detecting AI-Generated Text Using Comparative Embedding Methods with Different ML Classifiers
By: Maahum Khan

# 
Overview: 
- Detecting AI-generated text in a scientific context (i.e. research abstracts).
- Using 3 different embedding methods: 2 BERT models — Mini-BERT/Mini-LM, 394-dimensional embeddings, and Base BERT, 768-dim embedding — and TF-IDF vectorization. 
- Embedding models were each used and tested on 2 different datasets: Kaggle dataset (4100 samples) and Hugging Face dataset (used 14.3K samples). They were also evaluated on the full Hugging Face dataset, containing 28.6K samples (code on the bottom), but this was excluded from the report to maintain consistent experimental design and prevent redundancy (since results were almost identical to that of using the 14.3K samples). 
- Dataset names given in report and in code block where datasets are loaded
- For each embedding model + Dataset combination, feed embeddings into one of 4 different binary classifiers: Logistic Regression, Random Forest, SVM, and MLP.
- Visualization methods: t-SNE, UMAP, and PCA (top 3 components, in both 2D and 3D from all angles). Different UMAP and PCA hyperparameters were tested (different number of components for PCA and neighbours for UMAP), and t-SNE was done both with PCA (the standard) and without PCA (just to see). Note that the final report included PCA with 50 components and t-SNE with PCA. UMAP was excluded from final report due to 7-page limit and because it provided roughly the same information as the t-SNEs but was less clear. 
