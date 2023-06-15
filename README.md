#Web Scraping with Python: Scraping Data from a Website using BeautifulSoup.

[https://youtu.be/K5fSwn2W8lc](https://youtu.be/K5fSwn2W8lc)

Step 1: Install the Required Libraries:
The code begins by installing two libraries, 'requests' and 'bs4', using the pip package manager. These libraries are required for making HTTP requests and parsing HTML, respectively.

![image](https://github.com/anupamshrivastavaadm/Web-Scraping-with-Python/assets/118778677/a7f7967d-aef1-4e40-ad75-b16e69c6254a)

Step 2: Importing Libraries:
The necessary libraries, 'requests' and 'BeautifulSoup', are imported using the 'import' statements.

![image](https://github.com/anupamshrivastavaadm/Web-Scraping-with-Python/assets/118778677/b30fb7fe-a8fb-4a70-9f13-6e2eed78e26f)

Step 3: Getting the Webpage Content:
A URL link ("https://codingwithas.blogspot.com/") stored in a variable is assigned with the website's address that we want to scrape.
The 'get' function from the 'requests' library is used to retrieve the content of the webpage.
The 'content' attribute of the response object is accessed to get the HTML content of the webpage.
The webpage content is then passed to the BeautifulSoup constructor along with the parser ('html.parser') to create a BeautifulSoup object.

![image](https://github.com/anupamshrivastavaadm/Web-Scraping-with-Python/assets/118778677/b86ad35e-7621-428b-84d8-22a64eced902)

Step 4: Scraping Data from the Webpage:
The code identifies the specific data that needs to be scraped from the webpage using the 'find_all' method of the BeautifulSoup object.
In this case, it searches for all 'h3' elements with the class attribute 'post-title'.
The result is stored in the 'scrapedata' variable.

![image](https://github.com/anupamshrivastavaadm/Web-Scraping-with-Python/assets/118778677/deb892a1-8a09-4014-a177-82babe6d8f11)

Step 5: Printing the Scraped Data:
The code prints the scraped data by directly accessing the 'scrapedata' variable.
This will display the HTML tags along with the text content of the elements.

![image](https://github.com/anupamshrivastavaadm/Web-Scraping-with-Python/assets/118778677/209b19c6-7a08-4ae4-9c31-147db1742ea7)

Step 6: Cleaning the Scraped Data:
A list named 'scrapedata_list' is created to store the cleaned data.
A loop is used to iterate over each element in the 'scrapedata' list.
The 'text' attribute is accessed for each element to retrieve only the text content, excluding the HTML tags.

![image](https://github.com/anupamshrivastavaadm/Web-Scraping-with-Python/assets/118778677/601ee01a-747b-4668-81d2-db55292d284d)

The cleaned data is printed for each iteration.

The code essentially fetches the HTML content of a webpage, extracts specific data using BeautifulSoup, and then prints the scraped data after cleaning it.
