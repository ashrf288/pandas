
# pandas demo lab 


## Video Game Sales - Sales data from more than 16,500 games

In the `vg-stats` notebook answer the following questions/do the following tasks.
Note that the numbers quoted for sales are in the millions, and apply only for those games with over 10,000 sales.:

[x]Which company is the most common video game publisher?

Electronic Arts

[x]What’s the most common platform?

      DS 

[x]What about the most common genre?

      Action 

[x]What are the top 20 highest grossing games?
    

0                                       Wii Sports

1                                Super Mario Bros.

2                                   Mario Kart Wii

3                                Wii Sports Resort

4                         Pokemon Red/Pokemon Blue

5                                           Tetris

6                            New Super Mario Bros.

7                                         Wii Play

8                        New Super Mario Bros. Wii

9                                        Duck Hunt

10                                      Nintendogs

11                                   Mario Kart DS

12                     Pokemon Gold/Pokemon Silver

13                                         Wii Fit

14                                    Wii Fit Plus

15                              Kinect Adventures!

16                              Grand Theft Auto V

17                   Grand Theft Auto: San Andreas

18                               Super Mario World

19    Brain Age: Train Your Brain in Minutes a Day



[x]For North American video game sales, what’s the median?
   
   0.08


[x]Provide a secondary output showing ten games surrounding the median sales output assume that games with same median value are sorted in descending order?
    

[]For the top-selling game of all time, how many standard deviations above/below the mean are its sales for North America?

[]The Nintendo Wii seems to have outdone itself with games. How does its average number of sales compare with all of the other platforms?


[]Come up with 3 more questions that can be answered with this data set.

1- #question1
```
std_for_higher_sales=data['NA_Sales'].std()
std_for_higher_sales
```

2- #question2
`data[['Name','NA_Sales','Publisher']].groupby('Name').median()`


3- Question3
```
median_game_sales = data['Global_Sales'].median()
median_game_sales

highly_ten_games=data[data['Global_Sales']==median_game_sales].head(10)
highly_ten_games
```