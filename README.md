# Human Centered Data Science Project Pitch

Thomas Winegarden

An examination of data quality solutions in R based projects/repos (and possibly python) being applied prior to statistical analysis on Github.

### Motivation

I am interested in data quality issues that data scientists commonly encounter while doing analysis. I am also particularly interested in the solutions that analysts are coming up with to use code (specifically R or Python) to solve data quality issues. This is potentially useful from a practical perspective because it will enable knowledge sharing and even code sharing around common and specific data quality problems. This could help scientists develop accurate data cleaning solutions and share standardized code to agree on norms. I hope to understand firstly, the data quality issues that are easily and commonly solved across different types/industries of analysis projects. Secondly, I hope to learn about areas of data quality and data cleaning that are not easy, do not have an agreed upon method of solution, complex in nature, or have not been solved.

### Data Proposal

I plan to query or scrape github for public repos that use specific data quality libraries to apply data cleaning or data quality detection. I will first start with repos that use tidyr but may expand this to other libraries if the data set is too small or my bandwidth allows. The reason I am choosing to focus on github is I believe github is one of the largest collections of statistical analysis projects using R software. I plan to represent in this dataset column headers such as, university or origin, company of origin, license, tidyr Boolean, stringr Boolean, pylr Boolean, “Data Quality” Boolean, username, repo activity, stat analysis type. I do not have the dataset compiled at this time however I plan to utilize githubs search function in order to compile this set. https://help.github.com/en/github/searching-for-information-on-github/searching-code. Because I will not be running or using any of the code within these repos I hope that licenses will allow me to just observe their usage as a data point. However it will also be interesting analysis to attempt to scrape license type. This is also yet to be explored by myself. Ethical considerations include identifiable information of the author/user within my data set.

### Unknowns and Dependencies

It will be almost impossible to argue that this is a representative sample of data science projects as a whole. I will need to be clear about my search and query parameters while building the data set for analysis. 
This data may also be difficult to compile prior to analysis as it needs to be manually assembled and ironically will need data quality fixes and data cleaning of its own. That is to say a clean data set is not readily available and I have yet to find similar research or project research questions similar to the pitch I propose.
