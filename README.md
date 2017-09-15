# Explore weather trends.

## Introduction.
This project is my implementation of the _"Explore weather trends"_ project which is project 0 in the Udacity DataAnalyst Nanodegree program. Here is a [link](https://www.udacity.com/course/data-analyst-nanodegree--nd002) to the program. As I live in the Netherlands I will compare the global temperature data with that of a city in the Netherlands. 

## Step 1. Understanding the schema.
Before retrieving the data it is important to understand the schema of the database. It was given that the database consisted of three tables city\_list, city\_data, and global\_data. The scema was explored in the following manner.
Command:
```
SELECT * FROM city_list LIMIT 1;
```
Result:

| city	| country |
| ----- | ------- |
| Abidjan | Côte D'Ivoire |

Command:
```
SELECT * FROM city_data LIMIT 1;
```
Result:

| year | city | country | avg_temp |
| ---- | ---- | ------- | -------- |
| 1849 | Abidjan | Côte D'Ivoire | 25.58 |

Command:
```
SELECT * FROM global_data LIMIT 1;
```
Result:

| year | avg_temp |
| ---- | -------- |
| 1750 | 8.72 |

## Step 2. Retrieving the data.
### Selecting a city.
Now it is time to select a city from the Netherlands. First I wanted to know which cities from the Netherlands were available in the database.
Command:
```
SELECT * FROM city_list WHERE country = 'Netherlands'; 
```
Result:

| city | country |
| ---- | ------- |
| Amsterdam | Netherlands |

Hmm for obvious reasons I choose Amsterdam.

### Getting the starting point.
To find out the first year from which global data is available I used the following command. 

```
SELECT * FROM global_data ORDER BY year LIMIT 1; 
```
Result:

| year | avg_temp |
| ---- | -------- |
| 1750 | 8.72 |

This is the same result as I got from investigating the global_data schema above, so apparently the data was already ordered by year.

Now for Amsterdam
```
SELECT * FROM city_data WHERE city = 'Amsterdam' ORDER BY year LIMIT 1; 
```
Result:

| year | city | country | avg_temp |
| ---- | ---- | ------- | -------- |
| 1743 | Amsterdam | Netherlands |7.43 |

The results above mean that I can compare Amsterdam with global data from the year 1750.

### export to sheets

## Step 3. Visualize the data
### moving average
### plot

## Observations.