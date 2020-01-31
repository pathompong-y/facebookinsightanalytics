# facebook's Insight Analytics
This project is data analytics project that analyzes data from facebook insight of the page 'https://facebook.com/manudglom' to extract more insight guiding the influence factors of the page growth and how can we predit it.

It is analyzed by using Python 3 on Jupyter Notebook.

# The Objectives of this Project
Facebook Page Insights is the first stop tool for all of Facebook page admin to analyze and measure the performance of the content posted / published on the page. However, there are in-depth and page specific questions that facebook insight can't answer. For example, the metrics that influences the increment of the total page's like. Is it a set of 'Like, Comment, Share'? or Is it actually just 'Share'? or base on the average performance of the content, how can I predict the growth of the page? 

As I'm also running facebook fan page for my online comics (https://facebook.com/manudglom) and also curious about these, it drives me to go beyond the tool by extracting the data and do some analysis to answer my top 3 important questions as listed below.

1. What are the factors that influence new daily page like?
2. What are the approximated value of factors that influences the page like?
3. How can we predict daily page like when there is a new post published?

# How to run the notebook
- [Install Anaconda 3](https://www.anaconda.com/distribution/)
- Open Anaconda 3 console and create environment compatible with Python 3++ with the command:
`conda create -n <environment name> python=3`
- Activate the created environment with the command:
`activate <environment name>`
- Clone this project and all of the files to your local machine
- Open FB.ipynb, go thru the note and run the code to see the result

## Required Libraries
- pandas
- numpy
- matplotlib
- seaborn
- sklearn
- datetime

All of them will already bundled with Anaconda 3's Python environment or can be installed with the command `pip3 install <libraries name>`, if you install Python and Jupyter Notebook with other method.

## File Description
1. FB.ipynb : This is Jupyter Notebook file. Run this file to see analysis steps and result.
2. 2018-1.csv, 2018-2.csv, 2018-3.csv, 2019-1.csv, 2019-2.csv, 2019-3.csv : These are the post level data files.
3. Page 2020.csv : This is page level data file.
4. LICENSE : License note for this project.
5. README.md : This page.

# Result Summary
This is based on my facebook page's post data 2 years backward and page data 180 days backward from January 2020.

1. What are the factors that influence new daily page like?
> Post's Share, Like, Impression and Reach

2. What are the approximated value of factors that influences the page like?
> Like : 38-1,000 | Share : 1-40 | Impression : 0-40,000 | Reach : 0-25,000

3. How can we predict daily page like when there is a new post published?
> We can't predict directly now due to low datapoint of page & post combined.
However, we can predict "Share" from "Like" and "Impression" using linear regression with 85% R-Square.