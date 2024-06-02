# web_scraping
mars part 1
Import Necessary Libraries:

We imported the splinter library for browser automation and the BeautifulSoup library for parsing HTML.
Setup Browser:

We set the executable path for chromedriver and initialized a Browser object with Splinter.
Visit the Mars News Site:

We navigated to the provided Mars news site URL using browser.visit(url).
Create a BeautifulSoup Object:

We obtained the HTML content of the page using browser.html.
We created a BeautifulSoup object to parse the HTML content.
Extract All Text Elements:

We used BeautifulSoup to find all the elements containing the news articles using news_soup.find_all('div', class_='list_text').
Create an Empty List:

We initialized an empty list mars_news to store the extracted data.
Loop Through the Text Elements:

We looped through each news article element, extracting the title and preview text.
For each article, we created a dictionary with the keys 'title' and 'preview'.
We appended each dictionary to the mars_news list.
Print the List:

Finally, we printed the mars_news list to confirm the successful extraction of the data.
This process automates the task of visiting the Mars news website, scraping the titles and preview texts of news articles, and storing the data in a structured format. This is a fundamental web scraping task that can be adapted for different websites and data extraction needs.

Mars_Part_2

Setup: Imported necessary libraries (splinter, BeautifulSoup, matplotlib, pandas) and set up the Splinter browser.

Scraping: Visited the Mars Temperature Data website, scraped the data using Beautiful Soup, and created a Pandas DataFrame from the scraped data.

Data Cleaning and Analysis: Examined and converted data types as needed. Analyzed the data to answer questions such as the number of months on Mars, the number of Martian days' worth of data, the average low temperature by month, and the average pressure by Martian month.

Visualization: Plotted the average temperature and pressure by month to visualize trends in the data.

Conclusion: Estimated the number of terrestrial days in a Martian year based on observed periodicity in the temperature data.

Export: Saved the DataFrame to a CSV file for further analysis or sharing.

Cleanup: Ended the browser session.
