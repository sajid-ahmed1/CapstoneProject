# Capstone Project - Formula 1

## Motivation

The motivation for this topic and dataset was due to my interest in Formula 1. I have been watching Formula 1 on and off since 2009 when Jenson Button lifted the Championship trophy racing with Brawn GP and their infamous double diffuser. I look through the dataset that is published on Kaggle here: https://www.kaggle.com/datasets/rohanrao/formula-1-world-championship-1950-2020 but retrieved using Ergast API here: http://ergast.com/mrd/. As of 30th of December 2024, the Formula 1 has concluded for the year with the data updated monthly. I also posted a medium article about my findings here: 

## Findings

For this assignment, I have chosen my problem statement to be 
"How can we optimise the race strategy to target the highest place finish taking in factors such as tire degredation, position changes and race pace."

From my findings, I found a lot of events that happened in the actual race to reflect in the data. For example, when safety cars are out due to adverse weather conditions, the lap times would shoot up as the race pace is grinded to a slow walking pace to ensure maximum safety. I used two different models to predict lap times, Random Forest and Gradient Boost which have their own explanations of how the algorithms work in the notebook. From the results, the Random Forest model performed much better with 57% of the variance explained. The model in general is okay but can be improved upon with additional features such as driver charecteristics (such as form and position from within the season) and weather data. I also use GridSearchCV to find the best parameters after establishing that the Random Forest model provides significantly better results.

## Libraries Used

### Data Manipulation and Analysis:

pandas
numpy

### Machine Learning:

scikit-learn (sklearn)

### Data Visualization:

matplotlib
seaborn

### Files within repository

Capstone_Project.ipynb
This is where the code is stored with the markdown text to explain each graph and my understanding/thoughts. 

## Licensing, Authors and Acknowledgement

### Data Source
Kaggle Formula 1 World Championship (1950-2024) : https://www.kaggle.com/datasets/rohanrao/formula-1-world-championship-1950-2020

### Acknowledgements
Vopani: https://www.kaggle.com/rohanrao
Udacity: https://www.udacity.com

### License

MIT License
Copyright (c) [2024] [Sajid Ahmed]

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
