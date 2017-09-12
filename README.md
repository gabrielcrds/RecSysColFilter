# RecSysColFilter
A recommendation algorithm based on collaborative filtering, made with C++. 
This was a programming activity of a class that I attended in the beginning of 2017.
The theacher made a closed Kaggle competition for the class. <br />
<br />
To see it working, you must provide two input files. First the ratings.csv file, with the
ratings that you already have in the following sintax: <br />
<br />
UserId:ItemId,Prediction,Timestamp<br />
u0026762:i2171847,6,1362062307<br />
u0026502:i0444778,8,1362062624<br />
...<br />
u0004598:i1411238,6,1362062838<br />
u0031317:i1496422,7,1362063503<br />
<br />
Then, a target.csv file, containing the user and item you want predictions about:<br />
<br />
UserId:ItemId<br />
u0026762:i2171847<br />
u0026502:i0444778<br />
...<br />
u0004598:i1411238<br />
u0031317:i1496423<br />
<br />
After making the executable using the makefile, you should run: <br />
./recommender ratings.csv targets.csv > submission.csv<br />
The program will create the submission.csv file, in the folowing sintax: <br />
<br />
UserId:ItemId,Prediction<br />
u0026762:i2171847,6.1362062307<br />
u0026502:i0444778,8.1362062624<br />
...<br />
u0004598:i1411238,6.1362062838<br />
u0031317:i1496422,7.1362063503<br />


In the competition, my algorithm got a RMSE (Rooted Mean Squared Error) of 1.70, getting the fifth place.
