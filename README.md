# Explore weather trends.

## Introduction.
This project is my implementation of the _"Explore weather trends"_ project which is project 0 in the Udacity DataAnalyst Nanodegree program. As I live in the Netherlands I will compare the global temperature data with that of a city in the Netherlands. 

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
### sql
### export to sheets

## Step 3. Visualize the data
### moving average
### plot

## Observations.