# TidyR on Github, a Human Centered Data Science Final Project

Thomas Winegarden - HCDE 512 (Autumn 2019)

An examination of data quality solutions in R based projects/repos (and possibly python) being applied prior to statistical analysis on Github.

## INTRODUCTION

### Motivation

I am interested in data quality issues that data scientists commonly encounter while doing analysis. I am also particularly interested in the solutions that analysts are coming up with to use code (specifically R or Python) to solve data quality issues. This is potentially useful from a practical perspective because it will enable knowledge sharing and even code sharing around common and specific data quality problems. This could help scientists develop accurate data cleaning solutions and share standardized code to agree on norms. I hope to understand firstly, the data quality issues that are easily and commonly solved across different types/industries of analysis projects. Secondly, I hope to learn about areas of data quality and data cleaning that are not easy, do not have an agreed upon method of solution, complex in nature, or have not been solved.

### Data Proposal

I plan to query or scrape github for public repos that use specific data quality libraries to apply data cleaning or data quality detection. I will first start with repos that use tidyr but may expand this to other libraries if the data set is too small or my bandwidth allows. The reason I am choosing to focus on github is I believe github is one of the largest collections of statistical analysis projects using R software. I plan to represent in this dataset column headers such as, university or origin, company of origin, license, tidyr Boolean, stringr Boolean, pylr Boolean, “Data Quality” Boolean, username, repo activity, stat analysis type. I do not have the dataset compiled at this time however I plan to utilize githubs search function in order to compile this set. https://help.github.com/en/github/searching-for-information-on-github/searching-code. Because I will not be running or using any of the code within these repos I hope that licenses will allow me to just observe their usage as a data point. However it will also be interesting analysis to attempt to scrape license type. This is also yet to be explored by myself. Ethical considerations include identifiable information of the author/user within my data set.

### Unknowns and Dependencies

It will be almost impossible to argue that this is a representative sample of data science projects as a whole. I will need to be clear about my search and query parameters while building the data set for analysis. 
This data may also be difficult to compile prior to analysis as it needs to be manually assembled and ironically will need data quality fixes and data cleaning of its own. That is to say a clean data set is not readily available and I have yet to find similar research or project research questions similar to the pitch I propose.

## PROJECT PLAN

### Research Questions

Q1. Over the last year, what percentage of public R projects on Github are using tidyR for data manipulation of any kind? Is there a trend in growth or otherwise?

Q2. Of the 5 main tidyR function categories (Pivoting, Rectangling, Nesting, Splitting and Combining, Implicit to Explicit) what is the comparative usage breakdown?

Q3. Within each of the 5 main tidyR function categories, what are the most common functions being used?

Q4. Is there a correlation between use of Tidyr and use of other R packages or libraries.

Q5. Can it be determined by observing the repository’s description, readme, author, or base data what the industry or sector the project is associated with? What is the breakdown of sectors that can be determined.

### Ethical considerations of the above research questions

I do not believe the existence and ability to query public R based Github repos is an ethical problem in of itself however I can imagine a few ethical concerns that may surface during analysis.

The primary ethical concern is around including the author of the repository within the dataset. Though these are public repos, I already find it tempting to research the background of repo authors outside of what is provided on github. This is possibly breaching the privacy of the authors and I will initially attempt to determine without outside sources than github. I may then include identity links authors willing provide, followed by explicit public sources such as Wikipedia or public university pages.

Secondarily, there is ethical concern in observing public datasets with various licensing even though I will not be executing any of their code. I will do an examination of licenses within the ~100 subset I plan to narrow down in order to determine and expand on ethical or IP concerns in this area.

Finally, I imagine there could be public repos on github that may have sensitive data within them. These could be unintendedly been made public, made public nefariously, or possibly due to negligence. This will be difficult to detect initially but may arise in examination and attempts to answer question 5.


### Hypothesis

H1. However, I hypothesize that the percent of projects using tidyR is increasing. I’ve come up with hypothesis via person heuristic observation of my twitter feed.

H2. Rectangling is most popular and Nesting is least popular of the main 5 categories.

H3. 
1.	Pivoting: gather()
2.	Rectangling: unnest_longer()
3.	Nesting: unnest()
4.	Splitting and Combining: unite()
5.	Implicit to Explicit: drop_na()

H4. dplyr.

H5. These will be a difficult data points to procure from the dataset and may require manual work. I believe by narrowing down the analysis to about 100 projects I can determine with these fields what the sector associated with the project is. I hypothesis that academic related research in the field of Statistics and Social Sciences is the most common.

I would like to call out that these are mostly exploratory questions and my hypothesis are submitted as very broad guesses sometimes not based on even heuristic observation.

### Related Work

The closest related project that I have been able to find that helps to explore public repositories that use R on Github is actually published by R Studio itself. I’ll let the project description speak for itself, “This project uses githubs code and repository api to collect information about all github repositories that use R.” The project can be found here: https://github.com/hadley/r-on-github. Hadley Wickham is the owner of the repo and works as a Chief Scientist at rstudio. Part of my plan involves reaching out to him as I believe he is also a contributor to the tidyR and tidyverse packages. Below are some charts he has created comparing R Repos vs Packages.
 
 Link to image of graph showing R repos vs pkgs on github
- https://github.com/hadley/r-on-github/blob/master/github-repos.pdf

I plan to use some of the data Hadley Wickham has queried via the github API already but expand upon it in the direction of specific packages such as TidyR as my research questions outline. There is also opportunity to use his code base to query new more specific information from github which I see highly likely I use to narrow down my focus to 100 repos.

Unfortunately I have not found other analysis or research that is similar in scope to my project plan is it currently stands. I will continue to actively search for public research into the usage of tidyR, data quality methods in R, and R on github usage statistics and ideally expand this section.

### Methodology

Investigation via data exploration will begin primarily with compiling and filtering the R on github data to repos that use specific packages such as tidyR. The sub sectioning of these groupings will primarily include counting and averaging with groups. I plan to plot via timeseries line graphs as well as show breakdowns via pie charts and bar charts.

Correlation analysis should also be involved in order to answer which packages trend together and possibly to relate tidyR main function usage.

Overall this is mostly a comparative analysis and investigation of use of the tidyR library for data quality and data cleaning activities. I believe with basic methods of usage count comparisons and visualization of categorical comparisons I can drive understanding of the five initial research questions.

I do not plan to incorporate machine learning methods to this dataset at this time.

