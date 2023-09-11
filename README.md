# DC_project
Repo for UVA Distributed Computing Final Project on Spark, recommender system, and graphical neural nets



# Papers:
1. https://arxiv.org/pdf/1905.08108.pdf (important)
2. https://arxiv.org/pdf/2002.02126.pdf (important)
3. https://arxiv.org/abs/1905.07854
4. https://arxiv.org/abs/2306.02330
5. https://dl.acm.org/doi/abs/10.1145/3568953
6. https://arxiv.org/abs/1706.02263

# Helpful tutorial/github link:
1. https://medium.com/@shivanshsethi8821/knowledge-graph-attention-network-for-recommendation-4be007989076
2. https://github.com/pretrain/pretrain
3. https://medium.com/stanford-cs224w/recommender-systems-with-gnns-in-pyg-d8301178e377 (important)
4. https://www.kaggle.com/code/dipanjandas96/lightgcn-pytorch-from-scratch (important)
5. https://github.com/ztor2/lightgcn_recommender_pyg
6. https://github.com/HKUDS/GFormer

# Guangya's notes

1. As long as we have user interaction data (user/item/user's feedback on item), we can use graph to model the user-item interaction biparite graph and then use spark's  mllib and graphX functionality for a few baseline models. (SVD++/Pagerank/ALS)
2. There were some old GNN methods with extensive online reference (Light GCN) that have achived the state of arts results on the user-item interaction biparite graph recommendation task, so we can use the same data as above and make a comparsion (easy to explore).

So the problem settings:

Recommender systems

Graphs:

Nodes: Users, items

Edges: User-item interactions

Tasks:

Predicting the edge ratings. Metric: RMSE

Predicting edge existence. Metric: Recall@K

Data: For this task we can use the Steam Game data if we take the number of hours played as implicit feedback

3. The above two methods are outdated, and current ongoing research focuses on either how to include side information (embedding matrix/pre-training) or how to add transformer/attention mechnaisim in the graph model. If we want to do something solid and get exposed to the current research, we should probably try this(But it's time consuming and not too many things online we can refer to, and we need to think carefully about the data we used as well (I have seen people tried amazon/movie lens/Yelp dataset) ).



# 