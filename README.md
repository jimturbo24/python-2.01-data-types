# python-2.01-data-types

  1. Fork this repository
  2. Check out your fork
  3. Make a branch and switch to it
  4. Add your answers to this file, each one surrounded by triple backquotes, like so:
    ```
    This is my answer
    ```
  5. Commit your answers to your branch
  6. Push your branch to origin
  7. Do a Pull Request against `master` in your repository
  8. Merge the pull request.
  9. Paste the link to your repository in your assignment in online.theironyard.com

## Answers for "variables" below
1.  ```In [1]: taxRate = 8.25```

2.  ```In [8]: 45.60 * taxRate / 100
    Out[8]: 3.762```

3.  ```In [26]: item1 = 20.65

    In [27]: item2 = 34.65

    In [28]: item3 = 57.83

    In [29]: subTotal = item1 + item2 + item3

    In [34]: tax = subTotal * taxRate / 100

    In [35]: total = subTotal + tax

    In [36]: total
    Out[36]: 122.463225```

4.  ```In [37]: name = 'Jimmy'

    In [38]: name
    Out[38]: 'Jimmy'```

5.  ```In [39]: greeting = "Hey, How's it going?"

    In [40]: greeting
    Out[40]: "Hey, How's it going?"```

6.  ```In [41]: print(name + greeting)
    JimmyHey, How's it going?```

7.  ```In [46]: print(greeting + " " + name + " you owe me " + str(total) + " for the repairs I made to your car.")
    Hey, How's it going? Jimmy you owe me 122.463225 for the repairs I made to your car.```

## Answers for "lists and dictionary's" below

1.   ```In [1]: friends = ["Landon", "Ken", "Joe", "Brian", "Bill"]
        In [2]: friends
        Out[2]: ['Landon', 'Ken', 'Joe', 'Brian', 'Bill']    ```

2.   ```In [3]: states = ["Ohio", "Arizona", "California", "Texas"]
        In [4]: states
        Out[4]: ['Ohio', 'Arizona', 'California', 'Texas']```

3.  ```In [5]: zipPop = {"78249": 20000, "78258": 35000, "78229": 17000, "78216": 26000}
        In [6]: zipPop
        Out[6]: {'78216': 26000, '78229': 17000, '78249': 20000, '78258': 35000}```

4.   ```In [1]: zipPopYear = {"1990": {'78216': 16000, '78229': 7000, '78249': 10000, '78258': 25000}, "2000": {'78216':    26000, '78229': 17000, '78249': 20000, '78258': 35000}, "2010": {'78216': 36000, '78229': 27000, '78249': 30000, '78258': 45000}}
        In [2]: zipPopYear
        Out[2]:
        {'1990': {'78216': 16000, '78229': 7000, '78249': 10000, '78258': 25000},
        '2000': {'78216': 26000, '78229': 17000, '78249': 20000, '78258': 35000},
        '2010': {'78216': 36000, '78229': 27000, '78249': 30000, '78258': 45000}}```
5.   ```In [3]: date = {"month": 4, "day": 18, "year": 2016}
    In [4]: date
    Out[4]: {'day': 18, 'month': 4, 'year': 2016}```

6. ```I used a list and only entered my friends first names. Each item in a list is independent and can therefore be repeated as many times as necessary. Two entries of "John Smith" each get there own index assignment with a value of "John Smith".```

7. ```Two letter abbreviations are most often used in postal addresses, so if you were pulling data for an address your list should contain abbreviations. Most other uses of state names will likely use the full name. A dictionary might be the best way to model both names using the state name as a key and a list of the names as the value (ie. {"texas": ["TX", "Texas"]} ). All two letter abbreviations would match the state name given in the dictionary key ("AL" maps to the "alabama" key, "AR" maps to the "arizona" key).```

8. ```I used a string for the key and an integer for the value. I think of a zip code more as a name and less as a number, so I gave it a string value, whereas I think of population totals as numbers, thus I made it an integer. Making the key an integer wouldn't really change much, except if you were asking people to input a zip code, then you'd have to take an extra step to change the input from a string to an integer before querrying the dictionary.```

9. ```I used a string for the census year. It seems like one way of using the data isn't better than another. Looking up population of a zip code over time would require several querries, as would looking up population of all zip codes over time. However, looking up population of all zip codes over time would be cumbersome if all zip codes in the US were included in the dictionary.```

10. ```Using my data model, the values that comprise the data could be formatted according to the ISO 8601 standard. After all, the data stored in a dictionary is unordered anyway.```

## Answers for "data structures" below

1. ```In [1]: libraryBook = {"J. R. Tolken": ["Fellowship of the Rings", "The Two Towers", "The Return of the King"], "Arthur C. Clark": ["2001", "2010", "3001"]}
In [2]: libraryBook
Out[2]:
{'Arthur C. Clark': ['2001', '2010', '3001'],
 'J. R. Tolken': ['Fellowship of the Rings',
  'The Two Towers',
  'The Return of the King']}```

2. ```In [6]: pointsXY = {1: [3 ,5], 2: [7, 3], 3: [5, 1]}
In [8]: pointsXY
Out[8]: {1: [3, 5], 2: [7, 3], 3: [5, 1]}```

3. ```In [3]: profiles = {"Michelle": ["married", 36, "rice", "san antonio"], "Jason": ["single", 40, "utsa", "houston"]}
In [5]: profiles
Out[5]:
{'Jason': ['single', 40, 'utsa', 'houston'],
 'Michelle': ['married', 36, 'rice', 'san antonio']}```

4. ```In [9]: chessBoard = {1:[1,2,3,4,5,6,7,8], 2:[1,2,3,4,5,6,7,8], 3:[1,2,3,4,5,6,7,8]}
In [10]: chessBoard
Out[10]:
{1: [1, 2, 3, 4, 5, 6, 7, 8],
 2: [1, 2, 3, 4, 5, 6, 7, 8],
 3: [1, 2, 3, 4, 5, 6, 7, 8]}```

 5. ```In [12]: inmates = {1401:["Bob", "A1", 209, "blue"], 1402:["Tom", "C3", 175, "brown"]}
In [13]: inmates
Out[13]: {1401: ['Bob', 'A1', 209, 'blue'], 1402: ['Tom', 'C3', 175, 'brown']}```

6. ```To remove "Fellowship of the Rings" use: del libraryBook["J. R. Tolken"][0]. To add it back use: libraryBook["J. R. Tolken"][2] = "Fellowship of the Rings"```

7. ```To tell if a point is in pointsXY use: 1 in pointsXY```

8. ```I used a dictionary for my social media profile data and dictionary keys must be unique, thus there would have to be a way to modify the names of two people with the same name to make them unique. Then use the unique name as a key```

9. ```Since I used a dictionary to make my chessBoard, it does not suffer from the "mutable presto-chango" mentioned in the article.```

10. ```To remove inmate Bob use: del inmates[1401].```
