# RecSysColFilter
A recommendation algorithm based on collaborative filtering, made with C++.
This was a programming activity of a class that I attended in the beginning of 2017.
The theacher made a closed Kaggle competition for the class, and I got the fifth place.

To see it working, you must provide two input files. First the ratings.csv file, with the
ratings that you already have in the following sintax:

UserId:ItemId,Prediction,Timestamp\n
u0026762:i2171847,6,1362062307\n
u0026502:i0444778,8,1362062624\n
...
u0004598:i1411238,6,1362062838\n
u0031317:i1496422,7,1362063503\n

Then, a target.csv file, containing the user and item you want predictions about:

UserId:ItemId\n
u0026762:i2171847\n
u0026502:i0444778\n
...
u0004598:i1411238\n
u0031317:i1496423\n

After making it using the makefile, you should run: ./recommender ratings.csv targets.csv > submission.csv
The program will create the submission.csv file, in the folowing sintax: 

UserId:ItemId,Prediction\n
u0026762:i2171847,6.1362062307\n
u0026502:i0444778,8.1362062624\n
...\n
u0004598:i1411238,6.1362062838\n
u0031317:i1496422,7.1362063503\n


In the competition, my algorithm got a RMSE (Rooted Mean Squared Error) of 1.70, getting the fifth place.
