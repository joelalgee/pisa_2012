# PISA 2012 Data Exploration
Exploring and visualising PISA 2012 data, using Python

## Summary

[PISA](https://www.oecd.org/pisa/) is the OECD's Programme for International Student Assessment. PISA measures 15-year-olds’ ability to use their reading, mathematics and science knowledge and skills to meet real-life challenges. The [PISA 2012 database](https://s3.amazonaws.com/udacity-hosted-downloads/ud507/pisa2012.csv.zip) (>300MB) contains the full set of responses from individual students, school principals and parents for 2012. An [accompanying dictionary](https://s3.amazonaws.com/udacity-hosted-downloads/ud507/pisadict2012.csv) explains the dataset's variables.

In this exploration of the UK data I was interested in the effect of explanatory features - gender, month of birth, and family situation (father and mother at home or not, siblings at home or not) - on student mindset (sense of belonging, attitude towards school, perceived control, perseverance and openness for problem solving) and proficiency in mathematics, reading and science.

I cast a wide net with exploration of a large number of features, in an attempt to discover something with potential for an interesting multivariate analysis.

It should be noted that there are [specific requirements](https://www.oecd.org/pisa/data/httpoecdorgpisadatabase-instructions.htm) for analysing this dataset to ensure unbiased results. These include the application of weights for obtaining unbiased population parameter estimates, replicate weights for obtaining unbiased standard errors, and the use of a set of plausible values for the calculation of student proficiency estimates.

It should also be noted that the student mindset responses in particular cannot be regarded as independent of one another.

Therefore, while a thorough exploration would need to include tests for statistical significance, these will be omitted here as the calculations are rather complex, and outside the scope of this project.

## Package versions

* python 3.8.5
* numpy 1.20.1
* pandas 1.2.4
* matplotlib 3.3.4
* seaborn 0.11.2
* sqlalchemy 1.4.25

## Instructions

Store all files in the same folder, download and unzip data to this folder, and use Jupyter Notebook to open pisa_2012_exploration.ipynb

## Files

### pisa_2012_exploration.ipynb

Contains the step-by-step analysis and discussion as an interactive Jupyter Notebook.

### pisa_2012_exploration.html

Static HTML version of the above.

### pisa_2012_slide_deck.slides.html

A browser-based slideshow highlighting some findings from the exploration.

## Data

The data provided by PISA can be downloaded [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud507/pisa2012.csv.zip).

## Conclusions

Male students had, on average, a more positive mindset than female students, with exceptions in some areas. Male students seemed, on average, more proficient in mathematics and science, and less proficient in reading than female students.

Students with both mother and father at home had, on average, a more positive mindset than without both at home. They also seemed, on average, more proficient in mathematics, science and reading.

Students with siblings at home had, on average, a more positive mindset than those without. There was no difference in proficiencies in mathematics, science and reading.

Students born in the first third of the academic year had, on average, a more positive mindset than those born in the last third. They also seemed, on average, more proficient in mathematics, science and reading.
