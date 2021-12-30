# Collaborative-Filtering-Recommendation
Implemented and developed different algorithms for the purpose of movie recommendation through movie rating predictions

## Introduction

<p align = "justify">
In this project, we were supposed to implement and develop different algorithms for the purpose of movie recommendation through movie rating predictions. There were 6 main algorithms to implement. Out of the 6, four were user-based algorithms including a basic algorithm using cosine similarity, basic algorithm using Pearson’s correlation, an extended algorithm with inverse frequency and another extended algorithm with case amplification. In addition, item-based algorithm and finally our own algorithm. </p>

## Algorithms

<ul>
  
<li> User-based algorithms
  <ol>
  <li> User Based Collaborative Filtering: Cosine Similarity </li>
  <li> User Based Collaborative Filtering: Pearson's Correlation </li>
  <li> User Based Collaborative Filtering: Pearson's Correlation with Inverse User Frequency </li>
  <li> User Based Collaborative Filtering: Pearson's Correlation with Case Modification </li>
  </ol>
</li>
<li> Item Based Collaborative Filtering </li>
<li> Custom Algorithm </li>
  
</ul>

## Results

<p align = "justify">
The worst performing algorithm was using Pearson’s correlation with case amplification. I believe this is so because the case amplification didn't work well with this dataset. I also believe if we use inverse user frequency and then apply case modification, it would work better, though I didn't have time to try this experiment. Cosine Similarity on its own works relatively well, however, since it has its drawbacks, it doesn't have the best performance. Pearson’s correlation with IUF works better than Cosine and this is because Pearson’s correlation covers the issue of inverse relationship and IUF differentiates between the popularity of the movies which helps. Item-based doesn't do that well, probably due to the sparsity of the movie matrix, when we consider the movies as vectors. </p>

<p align = "justify">
The best performing algorithm was my algorithm which used cosine similarity, Pearson’s correlation and item-based prediction in one algorithm. I believe this works well because ensemble techniques work well and any issue that one similarity metric might have is covered by another metric. For example, cosine doesn't work well for inverse relationships, so Pearson’s correlation takes care of that. Both cosine and Pearson’s correlation won't consider the popularity of the movies, so adding IUF helps with that. Finally, similarity between the movies also helps in prediction and therefore adding item-based prediction improved the performance. Also, using adjusted cosine similarity will help in considering individual user bias. I believe since all these issues are addressed, the combination algorithm works best. </p>

