# Amazon Book Scraper

This Python script scrapes book information from Amazon, including the book's title, author, price, rating, reviews, and a link to the book's page. The script uses the BeautifulSoup library to parse the HTML content and stores the extracted data in a CSV file.

## Features

- Scrapes book titles, authors, prices, ratings, reviews, and product links.
- Loops through multiple pages to retrieve a larger dataset.
- Randomized sleep intervals to prevent blocking.
- Saves the scraped data into a CSV file (`amazon_books.csv`).

## Prerequisites

- Python 3.x
- Required Python packages (install via `pip`):
  - `requests`
  - `beautifulsoup4`

You can install the required packages with the following command:

```bash
pip install requests beautifulsoup4
```

## Usage
1) Clone the repository and navigate to the project directory:
   ```git clone https://github.com/CyberFantics/amazon-book-scraper.git
      cd amazon-book-scraper
   ```
2) Run the scraper:
   ```git clone https://github.com/CyberFantics/amazon-book-scraper.git
      cd amazon-book-scraper
   ```
  The scraped data will be saved in the `amazon_books.csv` file.

## Customization
You can modify the search keyword by updating the url variable. For example, change 'boiks' to your desired search query in the URL:
```url = f'https://www.amazon.com/s?k=books&page={page}&qid=1725444238&ref=sr_pg_{page}'
```

## Notes
- The scraper includes random delays between requests to avoid getting blocked by Amazon.
- Amazon may block requests if they detect too many in a short period.

## License
- This project is licensed under the MIT License. See the LICENSE file for more details.
