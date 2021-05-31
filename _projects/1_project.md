---
layout: post
title: Covid-19 Data scrapper
description: A script written to pull Covid-19 data directly from the JHU's Covid-19 Github repo
---

[Here](https://github.com/TemiPete/Covid19){:target="_blank"} is the repo for this fun project.

## Sometime in June...

Back in June 2020, when the Covid-19 pandemic was ravaging the world and many people had to [WFH](https://www.urbandictionary.com/define.php?term=WFH){:target="_blank"}, I thought I would put some R chops to practice. I was interested in understanding how infection and remission rates were going over time, i.e. if they were going up or going down. Naturally, I needed to pull the data. At that time, Johns Hopkins University (JHU), had set up a [dashboard](https://coronavirus.jhu.edu/map.html){:target="_blank"} showing infection rates across the world. Somehow, I couldn't get an API to pull the data from them, and I did not know of R packages already made to grab Covid-19 data in real time. 

So, I solved my problem in a crude manner. I found JHU's Github page where they saved daily cases of Covid-19 in a csv file. One can fork/clone this repo and grab the data (cloning the repo was my first attempt). But I found that doing this might not be efficient enough. Moreover, the files in the repo will get bigger over time, increasing the need for enough memory on a local computer for anyone who wanted to run my script. 

I decided to find a way to read the data directly from JHU's github page and save it in a csv file in a directory the user specifies. That is exactly what this script does. 

## Future Plans
I have decided to add more functionality to the script over time. 
- I want to make it run as a Shiny app. This way, anyone can pull the data of the country(-ies) they want, and visualize the data in interesting ways. 
- Afterwards, I want to add statistical functionality to the app. This way, one can calcuate summary statistic on the data and run a few statistical tests. 
- The success of the script is heavily dependent on JHU's Covid-19 github page. I should consider adding options in case something bad happens to that page. 
