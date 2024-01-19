# Udacity: Advanced Cleaning Project

> ### Project Parameters:

* Gather at least two datasets - successfully extract data using two different data gathering methods and combine the data to answer a research question.
    - NOTE: Three datasets were gathered using <ins>**web scraping</ins>,** <ins>**API</ins>,** and <ins>**direct download**</ins>
* Assess the data according to quality and tidiness metrics using both visual observations and coding, identify missing data, duplicate data, and any other issues concerning the data.
* Clean the data to solve the issues found in the assessing step.
* Update the data store with the cleaned data.
* Produce basic visualizations on the cleaned data, and answer a simple research question on the dataset.
    - NOTE: The primary focus of this project is **wrangling** and **cleaning** data, visualizations and conclusions are secondary and instead are the focus of a different project.

In the end, you will have completed a professional data-wrangling and cleaning process and be able to generate basic visualizations.

> ## Project Details

### Problem Statement

I'm exploring the relationship between CO2 emissions and average temperature on a per country basis per year. More specifically, I'll be looking at the world's two largest GDPs, USA and China; is there a positive correlation between CO2 emissions and temperature, i.e. as CO2 emissions increase, does the temperature as well?

### Dataset Sources

* The 1st dataset is from Global Monitoring Laboratory and contains historic data on 6 different gasses contributing to climate change. 
* The 2nd dataset is from Berkeley Earth and contains historic Earth temperatures for most of the world's countries.
* The 3rd dataset is from World Bank and contains various historic climate change metrics per country/per year. 

### Dataset 1
>    *Wrangle Method*: Web Scraping using BeautifulSoup
>
>       **Note: This dataset was under 500 rows and therefore didn't meet the project rubric for minimum datapoints, however since it's a good example of web scraping, the wrangling of this data is included in the Jupyter notebook.**
>
>    *Type*: .csv file
>
>    Dataset variables:
>
>    * Year: The year
>    * CO2: Carbon Dioxide
>    * CH4: Methane
>    * N20: Nitrous Oxide
>    * CFC: Chlorofluorocarbons
>    * HCFC: Hydrochlorofluorocarbons
>    * HFC: Hydrofluorocarbons

### Dataset 2
>    *Wrangle Method*: File was aquired using **Kaggle's** API
>
>    *Type*: .xls file (Microoft Excel)
>
>    Dataset variables:
>
>    * Year: The year
>    * Country name: Countries
>    * Series name: Contains different climate change variables
>    * 1990 - 2011: Values of CO2 listed under multiple years
>    * Other variables that are not necessary and will be handled in cleaning

### Dataset 3
>   *Wrangle Method*: Direct download
>
>   *Type*: .csv file
>
>   Dataset variables:
>
>    * dt: The year, including month and day
>    * Average Temperature: Temperature for that month and year in Celcius
>    * Country: Countries
>    * Other variables that are not necessary and will be handled in cleaning