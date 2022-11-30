# What is Web Scraping?

## Web Scraping

Web scraping is the process of extracting large amounts of data from a website in a short amount of time.

Step 1: Start by downloading the data from the site as turnstile data.

Always look up the information on the website to learn what information is legally able to be webscraped.

Step 2. Inspect the website to find the locations of links and files in the different levels of HTML tags.

Step 3. Import your libraries and set your URL to the website you want to access. An example of this is below:

```python
import requests
import urllib.request
import time
from bs4 import BeautifulSoup

url = 'http://web.mta.info/developers/turnstile.html'
response = requests.get(url)
```

Step 4. Parse the html so that we can work with a nicer nested data structure. Here is what that looks like.

```python
soup = BeautifulSoup(response.text, “html.parser”)
```

Step 5. Narrow your search down to locate the HTML tags you want to find.

```python
soup.findAll('a')
```

Step 6. Extract the link and test it out.

```python
one_a_tag = soup.findAll(‘a’)[38]
link = one_a_tag[‘href’]
```

Step 7. Save the link to a variable so that your requests can go through automatically.

```python
download_url = 'http://web.mta.info/developers/'+ link
urllib.request.urlretrieve(download_url,'./'+link[link.find('/turnstile_')+1:])
```

Step 8. Write a line of code tpo pause the requests so the site doesn't see you as a spammer and block your code. 

```python
time.sleep(1)
```

## Things I want to know more about

Are there limitations to types of data that can be scraped, or is it only based on HTML tag?

### Resources

[How to Web Scrape with Python in 4 Minutes](https://towardsdatascience.com/how-to-web-scrape-with-python-in-4-minutes-bc49186a8460)

[Build A Python App That Tracks Amazon Prices!](https://www.youtube.com/watch?v=Bg9r_yLk7VY)

### Links

- >[Advanced Software Development](README.md)
