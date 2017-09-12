# RecSysColFilter
A recommendation algorithm based on collaborative filtering, made with C++.
This was a programming activity of a class that I attended in the beginning of 2017.
The theacher made a closed Kaggle competition for the class, and I got the fifth place.

To see it working, you must provide two input files. First the ratings.csv file, with the
ratings that you already have in the following sintax:

UserId:ItemId,Prediction,Timestamp
u0026762:i2171847,6,1362062307
u0026502:i0444778,8,1362062624
...
u0004598:i1411238,6,1362062838
u0031317:i1496422,7,1362063503

Then, a target.csv file, containing the user and item you want predictions about:

UserId:ItemId
u0026762:i2171847
u0026502:i0444778
...
u0004598:i1411238
u0031317:i1496423

After making it using the makefile, you should run: ./recommender ratings.csv targets.csv > submission.csv
The program will create the submission.csv file, in the folowing sintax: 

UserId:ItemId,Prediction
u0026762:i2171847,6.1362062307
u0026502:i0444778,8.1362062624
...
u0004598:i1411238,6.1362062838
u0031317:i1496422,7.1362063503


In the competition, my algorithm got a RMSE (Rooted Mean Squared Error) of 1.70, getting the fifth place.
