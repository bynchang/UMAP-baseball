Uniform Manifold Approximation and Projection (UMAP) is a scalable manifold learning algorithm for dimension reduction and visualization. Its goal is to find a low-dimensional representation of the data while preserving the distance structure in the original space as much as possible. Mathematically, it does so by minimizing the fuzzy set cross entropy between the fuzzy topological representation of the data and that of the low-dimensional representation. The package's <a href="https://umap-learn.readthedocs.io/en/latest/">documentation</a> gives a clear tutorial on the theory behind it, while I also recommend reading the <a href="https://arxiv.org/abs/1802.03426">original paper</a>, which includes comparisons with other dimension reduction algorithms like PCA and t-SNE.

In this project, I utilized UMAP to learn a latent representation of the arsenals of the MLB pitchers in the 2019 season. The data is scraped from the baseball website <a href="https://baseballsavant.mlb.com/">Savant</a>, which records the release speed, horizontal and vertical movement of each pitch of each pitcher. After learning the latent representation of pitcher arsenal, I ran a clustering algorithm (HDBSCAN) and was able to detect pitcher clusters in the dataset.
