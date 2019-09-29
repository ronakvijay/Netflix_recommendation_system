# Netflix_recommendation_system

<img src='https://camo.githubusercontent.com/48bce498d9b0d5d4e45fa0dd366fa242490328a3/687474703a2f2f7777772e7465636873637269707432342e636f6d2f61646d696e2f55492f6173736574732f696d672f426c6f6773496d6167652f6e6574666c69782d712e6a7067'>

### Business Problem
Netflix is all about connecting people to the movies they love. To help customers find those movies, they developed world-class movie recommendation system: CinematchSM. Its job is to predict whether someone will enjoy a movie based on how much they liked or disliked other movies. Netflix use those predictions to make personal movie recommendations based on each customer’s unique tastes. And while Cinematch is doing pretty well, it can always be made better.

Now there are a lot of interesting alternative approaches to how Cinematch works that netflix haven’t tried. Some are described in the literature, some aren’t. We’re curious whether any of these can beat Cinematch by making better predictions. Because, frankly, if there is a much better approach it could make a big difference to our customers and our business.

Credits: https://www.netflixprize.com/rules.html

### Problem Statement

Netflix provided a lot of anonymous rating data, and a prediction accuracy bar that is 10% better than what Cinematch can do on the same training data set. (Accuracy is a measurement of how closely predicted ratings of movies match subsequent actual ratings.)

### Machine Learning Problem

#### Type of ML Problem
For a given movie and user we need to predict the rating would be given by him/her to the movie. 
The given problem is a Recommendation problem 
It can also seen as a Regression problem 

#### Performance metric 
- Mean Absolute Percentage Error: https://en.wikipedia.org/wiki/Mean_absolute_percentage_error
- Root Mean Square Error: https://en.wikipedia.org/wiki/Root-mean-square_deviation

#### Machine Learning Objective and Constraints 
- Minimize RMSE.
- Try to provide some interpretability.

### Final Results
<table>
  <tr><th>Model</th><th>RMSE</th><tr>
  <tr><td>knn_bsl_u</td><td>1.0651583775048283</td></tr>
  <tr><td>svd</td><td>1.06539583258785</td></tr>
  <tr><td>bsl_algo</td><td>1.0655294354066949</td></tr>
  <tr><td>knn_bsl_m</td><td>1.066111028261093</td></tr>
  <tr><td>svdpp</td><td>1.0664479484659375</td></tr>
  <tr><td>xgb_all_models</td><td>1.0750049828399206</td></tr>
  <tr><td>xgb_bsl</td><td>1.0804996202827688</td></tr>
  <tr><td>first_algo</td><td>1.0865153626345139</td></tr>
  <tr><td>xgb_knn_bsl</td><td>1.0893322610406004</td></tr>
  <tr><td>xgb_final</td><td>1.096271036373701</td></tr>
</table>
