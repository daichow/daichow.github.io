---
layout: post
title:  "Covid-19 Global"
date:   2020-07-07
excerpt: "Get trustworthy current international facts and figures on Covid-19."
feature: https://user-images.githubusercontent.com/33791954/107156313-a9f80700-694b-11eb-9441-da91b9d893ab.jpg
tag:
- python 
- qt
- webscraping
- pandas
- matplotlib
project: true
---
<a href="https://github.com/mahirchow/COVID-19-GLOBAL" class="btn btn-info">Visit Github Repo</a>
<a href="https://devpost.com/software/covid-19-global" class="btn btn-info">Visit Devpost</a>
# Inspiration:

Our idea was brought about by the need to address the concerns that we share about the ongoing Coronavirus pandemic. Particularly, we felt concerned with the spread of information. Among the innumerous online sources which cover Covid-19 material, it is sometimes difficult for the average person to find the exact information they want or know whether it is always coming from a trusted news source. With this in mind, we decided to create our own platform for Covid-19 information that would provide current and trustworthy facts and figures.

<iframe width="560" height="315" src="https://www.youtube.com/embed/xbPZWd21G2g" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## What it does:

Our project is a desktop application which begins by displaying the current Covid-19 values for the World. These include the total number of cases and deaths, as well as the new number of cases and deaths for the current day. The user then has the option to type into a search bar the name of the country they wish to receive more specific information on. The application would then direct to a new screen where the country flag is generated along with the current Covid-19 facts, health statistics, and demographic values for that country. Furthermore, the user can click on any on the daily Covid-19 values to be redirected to another screen which displays a graph of all recorded values for the country since the beginning of the pandemic. It is important to note that all information is taken directly from a regularly updated online database which gathers its information from health and government agencies such the European Centre for Disease Prevention and Control, UN, and World Bank.

## Featured Images of Project
![gallery1](https://user-images.githubusercontent.com/33791954/107155287-9d70b000-6945-11eb-9fa1-a39f50888760.jpg)
*Figure 1: The initial home screen*
<br><br>
![gallery2](https://user-images.githubusercontent.com/33791954/107155289-9ea1dd00-6945-11eb-9932-6996be54440b.jpg)
*Figure 2: After searching up a specific country name*
<br><br>
![gallery3](https://user-images.githubusercontent.com/33791954/107155290-a06ba080-6945-11eb-895e-7fa4fa3bcb93.jpg)
*Figure 3: Data visualization graphs for each covid-19 fact*
<br>

## How we built it

We used various types of libraries and processes to aid in our program's back-end. Requests was used extensively to retrieve data from the web in various formats such as json or html. The json was then dumped and formatted into a json file called **data.json** and was then parsed later using the Pandas library to create dataframes for our data. We created various functions such as downloader, updater, and loader functions that deal with our data. We also created functions that manage our temporary files by efficiently deciding when to retrieve files from the web. All of this was then turned into a module called **covid_data.py** that could be imported into the main python file that runs the program.

As for our front-end, we used PyQt5 as our framework for our GUI.  We started of by templating and prototyping with the Qt Designer application so that we had a foundation to begin building our application upon. Once we were satisfied with a template, we converted it to python, and added more features to it later on. This code was then turned into a module called **design.py** that could be imported into the main python file that runs the program.

In our main python file, we created functions that could dynamically alter widgets in layouts as well as update values in them. We also used this file to bind buttons and labels to events and functions. The app's entry point starts from this python file.

## Challenges we ran into

Matplotlib and pandas were libraries that seemed to us to have a major learning curve. We had challenges understanding how the library and its classes worked.

We had issues integrating matplotlib with pyqt5. It was difficult to embed the plots into the layouts within the qt GUI.

## Accomplishments that we're proud of

We were able to make a project that was able to satisfy all of our initial goals.

Able to gather Covid-19 data from trustworthy sources

Allow user to search which country they want to receive data from

Created clear and organized user interface for users to view information

Able to generate graphs based on gathered data
 
## What we learned

We were able to learn about many different data science libraries and also got a bit of experience on how to use parts of it. 

This hackathon also gave us the opportunity to force ourselves to go outside of our comfort zone and tackle new things in python and data management. 

## What's next for Covid-19 Global

We would like to speed up our application significantly by getting rid of excess nested function callings in our code as well as redundant variables. 

As well, in the future, we would like to package this application to be easily distributable to users of all major operating systems.

## In order to run this code until further updates, please do the following:

**The following packages must be installed for this project to work:**
* bs4
* requests
* pycountries
* pyqt5
* matplotlib
* pandas
* datetime
* qtmodern
* re
* os
* time
* json

**afterwards, do the following command in terminal/cmd in the folder directory:**

* python main.py
OR
* python3 main.py
