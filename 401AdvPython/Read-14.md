## Web Scraping

### Web Scrape with Python
[Web Scrape with Python in 4 minutes](https://towardsdatascience.com/how-to-web-scrape-with-python-in-4-minutes-bc49186a8460)

* **Web scraping** is a technique to automatically access and extract large amounts of information from a website, which can save a huge amount of time and effort.

* Read through the website’s Terms and Conditions to understand how you can legally use the data. Most sites prohibit you from using the data for commercial purposes.

* Make sure you are not downloading data at too rapid a rate because this may break the website. You may potentially be blocked from the site as well.

* It is important to understand the basics of HTML in order to successfully web scrape.


### What is Web Scraping?
[What is Web Scraping?](https://en.wikipedia.org/wiki/Web_scraping)

* Scraping a web page involves fetching it and extracting from it. 
   - Fetching is the downloading of a page

* Web scraping is the process of automatically mining data or collecting information from the World Wide Web.

* The simplest form of web scraping is manually copying and pasting data from a web page into a text file or spreadsheet

* Static and dynamic web pages can be retrieved by posting HTTP requests to the remote web server using socket programming.

* Many websites have large collections of pages generated dynamically from an underlying structured source like a database. Data of the same category are typically encoded into similar pages by a common script or template. In data mining, a program that detects such templates in a particular information source, extracts its content and translates it into a relational form, is called a **wrapper**.

* some semi-structured data query languages, such as XQuery and the HTQL, can be used to **parse HTML pages** and to retrieve and transform page content.

* Languages such as Xpath can be used to parse the resulting DOM tree.

[How to scrape websites without getting blocked](https://www.scrapehero.com/how-to-prevent-getting-blacklisted-while-scraping/)

* Web scraping is a task that has to be performed responsibly so that it does not have a detrimental effect on the sites being scraped.

* Basic Rule: “Be Nice”, An overarching rule to keep in mind for any kind of web scraping is
BE GOOD AND FOLLOW A WEBSITE’S CRAWLING POLICIES

* the web scraping best practices you can follow to avoid getting web scraping blocked:

   - Respect Robots.txt, It has specific rules for good behavior:
      - how frequently you can scrape
      - which pages allow scraping, and which ones you can’t
      
* since most sites want to be on Google, arguably the largest scraper of websites globally, they allow access to bots and spiders. 

* Here are a few easy giveaways that you are bot/scraper/crawler :
   - Scraping too fast and too many pages, faster than a human ever can
   - Following the same pattern while crawling.
   - Too many requests from the same IP address in a very short time
   - Not identifying as a popular browser. You can do this by specifying a ‘User-Agent’.
   - using a user agent string of a very old browser

* When scraping, your IP address can be seen. A site will know what you are doing and if you are collecting data. They could take data such as – user patterns or experience if they are first-time users.

* Multiple requests coming from the same IP will lead you to get blocked, which is why we need to use multiple addresses. 