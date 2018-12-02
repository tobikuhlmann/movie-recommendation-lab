# Movie-recommendation-lab
UMass STAT535 Project - Movie recommendation

## Presentation
- Slide 1: Project proposal
  - Real world recommendation pipeline like it can be used on a website
  - Goal: Build python class which gives you recommended movies for a user
- Slide 2: Approach
  - Flow chart of pipeline (three user profile qualities -> three recommender systems (simple classification algo, content-based filter, collaborative filter)
- Slide 3: Methods (Not enough time to explain, formulas can be handled as backup)
  - Simple: Gradient Boosting Classifier (Boosted, penalized random forest) as black box from sklearn
  - Content-based recommender
  - Collaborative recommender
- Slide 4: Evaluation problematic
  - Simple and collaborative can predict user ratings
  - Not possible for content-based recommender -> No combined evaluation of our system possible
  - Possible solution: Give recommendations and catch feedback from users (how it would work in real-world)
- Slide 5: Summary
  - Different recommender systems for different users helpful, dependend on how good user profile
  - Evaluation hard at the beginning, need user feedback
  - Large datasets necessary


## Literature

- https://users.ece.cmu.edu/~dbatra/publications/assets/goel_batra_netflix.pdf
- http://delivery.acm.org/10.1145/1460000/1454012/p11-park.pdf?ip=72.19.68.210&id=1454012&acc=ACTIVE%20SERVICE&key=73B3886B1AEFC4BB%2EB478147E31829731%2E4D4702B0C3E38B35%2E4D4702B0C3E38B35&__acm__=1543416754_7f92e0642e26e7ea732886879096c704
- https://www.kaggle.com/prajitdatta/movielens-100k-dataset/kernels
- https://medium.com/@james_aka_yale/the-4-recommendation-engines-that-can-predict-your-movie-tastes-bbec857b8223
- https://www.kaggle.com/c/predict-movie-ratings
- https://cseweb.ucsd.edu/classes/wi17/cse258-a/reports/a048.pdf
- https://github.com/neilsummers/predict_movie_ratings/blob/master/movieratings.py
- https://medium.com/@connectwithghosh/recommender-system-on-the-movielens-using-an-autoencoder-using-tensorflow-in-python-f13d3e8d600d
### A few more
- https://sci2s.ugr.es/keel/pdf/specific/congreso/xia_dong_06.pdf (Uses SMV for classification, then MF for recommendation)
- https://www.kaggle.com/rounakbanik/movie-recommender-systems (Employs at least three Modules for recommendation)
- http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.703.4954&rep=rep1&type=pdf (Close to what we need, but a little too involving)
- https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0165868 (Uses SVM and correlation matrices...I have already tried the correlation approach, looks quite good, but how to quantify accuracy?)
- https://www.quora.com/How-do-we-use-SVMs-in-a-collaborative-recommendation (A good thread on SVM)
-http://www.quuxlabs.com/blog/2010/09/matrix-factorization-a-simple-tutorial-and-implementation-in-python/ (A good tutorial on matrix factorizasion)

## Milestones
- November 14th
  - Second dataset ready
  - Look at scikit learn template
  - Start master tree in github
 
 - After Thanksgiving
   - Preprocessing
     - Missing Values
     - Outliers
     - Standardized variable names
     - Encode qualitative / categorical variables
     - Data Reduction: Variable selection

   - Classifiers to start with: 
     - Decision Trees (Random Forest) (Scott)
     - SVM (Sixtus)
     - Gaussian Naive Bayes (Tobi)



## A very usful git reference
http://rogerdudler.github.io/git-guide/

## Scicit-learn template
Our class should look like that and implement the same methods (fit, predict)

- http://contrib.scikit-learn.org/project-template/template.html
- https://github.com/scikit-learn-contrib/project-template/blob/master/skltemplate/_template.py


## Possible Second data sets
- German credit data: https://archive.ics.uci.edu/ml/datasets/statlog+(german+credit+data)

##### Patrick's comments 11/9

- Goal: Build a small real world deployment pipeline like it can be used in netflix / amazon 
- build / test with movie recommendation data set (model fitting, data preprocessing, evaluation)
- Show that it also works with another dataset like product recommendation
 - Find data on UCI repo, kaggle, google search 

- Use scikit learn estimation: https://github.com/scikit-learn-contrib/project-template



