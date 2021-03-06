# Is Alex Ovechkin the National Hockey League's Best Goal-Scorer?
<b> by Clifton Saul

## Repo Contents & Navigation
* <b> [skater_stats.csv](https://github.com/cmszip/DATA601-Assignment1/blob/master/skater_stats.csv) </b> - dataset of NHL player stats dating from 1940 to 2018. The raw dataset can be found on the [Inalitics website](http://inalitic.com/datasets/nhl%20player%20data.html). This was sourced from [Hockey-reference](https://www.hockey-reference.com/), which is a repository of hockey statistics.<br>
* <b> [Notebook](https://github.com/cmszip/DATA601-Assignment1/blob/master/DATA%20601%20-%20Assignment%201%20-%20Ovechkin.ipynb) </b> - Jupyter Notebooks was used for this project. 'DATA 601 - Assignment 1 - Ovechkin' is the Jupyter Notebook containing the data preparation, cleaning, and exploratory data analysis. <br>
* <b> [README.me](https://github.com/cmszip/DATA601-Assignment1/blob/master/README.md) </b> - description and overview of the project, including its objectives, process, and results.
* <b> [License.txt](https://github.com/cmszip/DATA601-Assignment1/blob/master/License.txt) </b> - MIT license and copyright

## Motivation

Since his arrival in the NHL in the 2005-2006 season, Alex Ovechkin has been one of the league's most skilled and discussed players. This has also welcomed debate over whether he or another player is the best in the league. Given that what is best is often a subjective discussion, there is often more punditry involved than data analysis.

## Goal

Given the above motivation, the goal of this project is to determine if Ovechkin is the best at a particularly important skill: scoring goals. This project uses data analysis of NHL player stats to determine if Alex Ovechkin is the NHL's best goal scorer, and if so, why that is. Particular attention is paid to metrics such as goals per game, shooting percentage, and total shots.

## Data Overview

An original csv file of NHL player stats dating from 1940 to 2018 was used. This dataset includes:
  * 37,825 rows
  * 29 columns:
    * Column datatypes:
      * float64: 6
      * int64: 3
      * object: 20

This dataset was altered to include the following:
  * 28,554 rows
  * 12 columns
    * Column datatypes:
      * float64: 4
      * int64: 3
      * object: 5

## Data Limitations & Concerns

A limitation of the data is that not all hockey statistics have been historically tracked. While data metrics such as shots have been tracked for the last few decades (and the entirety of Ovechkin's career), they were not historically tracked in the early years of the NHL. This leads to many null values in the dataset. After alterations to the dataset, this most notably impacted the column for shots ('S') and shooting percentage ('S%'). 

This leads to an additional limitation: an assumption within the data set regarding null values was made. Many of the columns were listed as object datatypes when they should have been integers or floats. The original csv file often had a value of ' - ' in columns that were full of numerical values for goals, assists, etc. While it is easy to infer that the intention of ' - ' (and thus the resulting null value) is a 0, given that many players do not score goals or meet other metrics, it is still an assumption that was made.

Additionally, a number of rules changed at the start of Ovechkin's career. The NHL cancelled its 2004-2005 season due to a labor dispute, and when the league returned to play in Ovechkin's first season, they made changes to some of the rules of play. This makes comparisons between Ovechkin and some of hockey's all-time greats more difficult to make. As a result, this project will focus more on Ovechkin and his peers, particularly concurrent star players, which are easier comparisons to make.

## Summary & Conclusion

Ovechkin scores approximately 0.462 more goals per game than his peers and 0.439 more goals per game than the average NHL player since 1940. We also found that Ovechkin's shooting percentage is 2.544% higher than other forwards in the NHL, but in line with other NHL superstar players, so it is reasonable. Instead, where Ovechkin far exceeds other players is in his total shots. Ovechkin is able to shoot the puck far more often than even other NHL superstars. 

This leads us to the conclusion that yes, Ovechkin is the NHL's best goal-scorer because he is the best at generating shots while maintaining an above average shooting percentage. This leads to him having the highest goals per game, even when compared to other NHL superstars.

---

## Contributors

Clifton M Saul Jr.

---

## [License & copyright](https://github.com/cmszip/DATA601-Assignment1/blob/master/License.txt)

© Clifton M Saul Jr.
