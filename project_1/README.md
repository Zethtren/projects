# Project 1: SAT and ACT Statistics, Summaries and, Expectations

### Overview:
In this project I will clean, explore, analyze, and present data from the the 2017 and 2018 SAT's and ACT's. I will go through the python coding required to import, extract and, process the given Dataset. I will then extract information from this data given and use that data to generate a presentation.

### Datasets:

#### Provided Data:

In the attached files there are 4 given datasets:

- [2017 SAT Scores](./data/sat_2017.csv)
- [2017 ACT Scores](./data/act_2017.csv)
- [2018 SAT Scores](./data/sat_2018.csv)
- [2018 ACT Scores](./data/act_2018.csv)

This data represents the scores and participation rates of each individual state organized by test and year.

#### Additional Data:

For the purpose of further exploration the following sites were used to understand and extract meaning from the trends recognized in the provided data.

- [Information and map for mandated testing policies by state](https://www.edweek.org/ew/section/multimedia/states-require-students-take-sat-or-act.html)
- [Minnesota Education Policy](https://education.mn.gov/MDE/dse/cte/data/)
- [Delaware Education Policy](https://www.doe.k12.de.us/Page/2425)
- [Massachusetts Education Policy](http://www.doe.mass.edu/frameworks/current.html)
- [Nevada Education Policy](http://www.doe.nv.gov/State_Board_of_Education/)

### Data Cleaning and Visualization:


Using Jupyter Notebook I processed and analyzed the datasets provided. First I imported the data and cleaned to remove incomplete or incorrect data. After the data was cleaned I combined the data into .csv files by year and then 1 single .csv file merged by state.

After merging the data I used Seaborn's pairplot to quickly check for correlations in the data. Tableau was then used to display that data through chloropeth maps, which will be seen in the presentation.


- [Jupyter Notebook](https://git.generalassemb.ly/hbova/project_1/blob/master/code/SATACTExploration.ipynb)

- [2017 Data](https://git.generalassemb.ly/hbova/project_1/blob/master/code/combined_2017.csv)

- [2018 Data](https://git.generalassemb.ly/hbova/project_1/blob/master/code/combined_2018.csv)

- [All Merged Data](https://git.generalassemb.ly/hbova/project_1/blob/master/code/completesactact.csv)

### Further Research:

After trends were established by scatterplot correlations I conducted a deeper research into individiual state policies. I observed for trends which will be covered in detail in the presentation

### Presentation:

A presentation was constructed using Tableau for visualizations and Google slides for presentation.

- [Presentation](https://docs.google.com/presentation/d/1kPXkKuIXsLk4whnlASpNZ3Im5Bx7ibguIG1MEgeclLk/edit?usp=sharing)