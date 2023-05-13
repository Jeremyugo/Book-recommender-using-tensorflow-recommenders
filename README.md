## Book-recommender-using-tensorflow-recommenders

This repository contains a machine learning project that utilizes TensorFlow Recommenders to build a book recommender system. The system leverages the power of deep learning and recommendation algorithms to suggest personalized book recommendations based on user preferences.<br/>

![image](https://github.com/Jeremyugo/Book-recommender-using-tensorflow-recommenders/assets/36512525/5ba83000-e883-4cbd-96bf-3320223f1b1c)
<br/>

#### Packages used for this project include:
- Tensorflow
- Keras
- Tensorflow recommenders
- Numpy
- Pandas
- Pyinputplus
<br/>

#### Data
The [data](https://github.com/caserec/Datasets-for-Recommender-Systems/tree/master/Processed%20Datasets/BookCrossing) used for this project was gotten from GitHub. The Book Crossing dataset were collected by Cai-Nicolas Ziegler in a 4-week crawl (August / September 2004) from the Book-Crossing community with kind permission from Ron Hornbaker, CTO of Humankind Systems.
<br/>

#### Evaluation
The model performed well on the test set, with the following metrics:
- Root mean square error: 1.887
- Top 1 accuracy: 29.39%
- Top 5 accuracy: 70.72%
- Top 10 accuracy: 79.04%
- Top 50 accuracy: 88.24%
- Top 100 accuracy: 89.39%
<br/>

#### Model Architecture
The recommendation model was built using TensorFlow Recommenders and consists of several dense layers and a Deep & Cross layer for feature crossing. The model is also capable of performing retrieval and ranking tasks which are the main components of real-world recommendation systems. The model can include embedding layers to represent user id, user age, book author and book title information. After training the model, a custom function `Recommend()` which takes user input and validates them against a other custom functions was created. This function performs the retrieval of books that align with the user's interests and outputs them in the order of their ranking.<br/>
<br/>
#### `UserModel()`
![usermodel](https://github.com/Jeremyugo/Book-recommender-using-tensorflow-recommenders/assets/36512525/9966ea87-dadd-4352-a356-db2913bd6093)
<br/>

#### `TitleModel()`
![titlemodel](https://github.com/Jeremyugo/Book-recommender-using-tensorflow-recommenders/assets/36512525/22c56045-509f-44a6-950b-6ee64654bd59)
<br/>

#### `FullModel()`
![fullmodel](https://github.com/Jeremyugo/Book-recommender-using-tensorflow-recommenders/assets/36512525/2b7a0e76-fbf3-4ffe-b7aa-ccff61d09f5c)
<br/>
