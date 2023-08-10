
# Aspect-Based Sentiment Analysis for Product Reviews

This Python script performs Aspect-Based Sentiment Analysis on product reviews scrapped from a website. It uses the `requests` library to fetch review data, `BeautifulSoup` for parsing HTML, `pandas` for data manipulation, and the Hugging Face `transformers` library for sentiment analysis and aspect classification.

## Prerequisites

Make sure you have the required libraries installed before running the script. You can install them using the following command:

```bash
pip install requests beautifulsoup4 pandas transformers
```

## Usage

1. Run the Colab note `main.ipynb`.
2. The script will scrape reviews from multiple pages of a product review website and save them to a CSV file named `CSV_OUT.csv`.
3. Sentiment analysis will be performed on each review using the Hugging Face `sentiment-analysis` pipeline.
4. Aspect classification will be performed on each review using the Hugging Face `zero-shot-classification` pipeline.
5. Aspect-based sentiment scores (positive and negative) will be calculated and added to the DataFrame.
6. The final DataFrame will be saved to `CSV_OUT.csv` with additional columns for aspect-based sentiment scores.

## Configuration

You can customize the script by modifying the following variables:

- `aspects`: A dictionary containing aspects to be analyzed along with their corresponding rank.
- `review_pages`: The number of review pages to scrape from the product review website.
- `max_text_length`: Maximum number of characters to use for sentiment and aspect classification.
- `csv_file_name`: Name of the output CSV file.

## Notes

- The script assumes that the website structure remains consistent and uses class names for scraping.
- Ensure that you respect the website's terms of use and scraping policies.

## Disclaimer

This script is provided for educational purposes and may require modifications to work with different websites or to address changes in libraries. The effectiveness of sentiment analysis and aspect classification may vary based on the underlying models used by Hugging Face.

**Use this script responsibly and respect website terms and policies.**

---

For more information and updates, feel free to contact the script author: [Ahmad Muhammad](mailto:ahmadmuhammadgd@gmail.com).
