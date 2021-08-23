# Webscraping Wikipedia Country Demographics
Web-scraping Wikipedia pages using Requests and Beautiful Soup and Pandas

You can better view the Jupyter notebook [here on Jovian.](https://jovian.ai/samantha-roberts/webscraping-wiki-country-demographics) 
***

I am very interested in geography and learning statistics about other countries in the world.  I frequently use Wikipedia to quickly get this information.  **In this project I will show how I used Python programming libraries (Beautiful Soup, Requests, Pandas) to gather demographic information about the many countries of the world by scraping Wikipedia web pages.**

Wikipedia is a collaborative online publicly editable encyclopedia.  It is the largest and most-read reference work in history, and consistently one of the 15 most popular websites visited[Ref](https://www.economist.com/international/2021/01/09/wikipedia-is-20-and-its-reputation-has-never-been-higher). Though anyone in theory can edit a wiki page, there are some light governances in effect that attempt to suggest how some pages are structured.  One of the ways that this can be done is via [WikiProjects](https://en.wikipedia.org/wiki/Wikipedia:WikiProject), where a group of contriburors attempt to work together as a team to improve a topic, often by attempting to standardize it to some extent.  ["Demographics"](https://en.wikipedia.org/wiki/Wikipedia:WikiProject_Demographics) is one such WikiProject.  In this project, each country has a demographics page, and many of these pages have a table that would be displayed in the right hand colum of each country page.  This table contains information on things like population breakdown by race, sex, religion, population density, birth and death rate, language, government type and so forth. **It is this demographics summary table that this project attempts to find and scrape for each country of the world.**

<img src="https://i.imgur.com/T9OASLH.png" width="80%">.

## Project Steps:

1. **Scrape the main demographics page to build a list of countries and their Wiki-links**
    - Using the python Requests and Beautiful Soup librarys we will scrape the [Wikipedia page](https://en.wikipedia.org/wiki/List_of_countries_and_dependencies_by_population) that lists the links of all county wiki pages
    - Parsing the HTML data we will make a list of dictionaries, 1 dictionary for each country that contains the country name and the link to the individual page
    - Using Pandas, we will read this data into a CSV file  


2. **Scrape individual country pages for their demographics**  

    - Read the countries and links into a dataframe using Pandas
    - Crawl the links in the CSV file and see how many country pages have the table I am trying to scrape
    - Write code specific to the majority of demographics page tables to scrape the data I want
    - Handle instances where the relevant tables do not exist in the demographics page  


3. **Clean the data scraped**  

    - Look at the data in Pandas and see if there is some 1st order way to clean the data further
    - Write the demographics info to a CSV file











