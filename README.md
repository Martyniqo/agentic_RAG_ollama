# Reddit Real Estate Insights with Ollama

This notebook leverages the Reddit API to gather and analyze discussions related to house prices in the United Kingdom. It performs a search within specific subreddits, retrieves posts discussing real estate, and extracts top comments to generate insights.

⚠️ **Note**: This project is designed to explore the capabilities of **open-source lightweight models** like **Mistral-NEMO**. While it functions as intended, it's still experimental and may require adjustments for more complex tasks. For example, integrating a larger model could offer deeper contextual understanding or more nuanced sentiment analysis. However, the focus here is on showcasing what can be achieved using smaller, efficient models for local and resource-constrained environments. 

## Features

- **Reddit API Integration**: Fetches posts from the `HousingUK` subreddit.
- **Custom Search**: Search functionality retrieves and ranks posts based on keywords like "house prices," "apartment prices," and "real estate."
- **Comment Analysis**: Extracts and formats top comments (based on upvotes) for deeper insights into real estate trends.
- **Natural Language Response**: Generates a natural language answer summarizing the findings, including average prices and locations if available.

## Requirements

- `praw`
- `pydantic`
- `datetime`

## How to Use

1. Clone this repository.
2. Install dependencies:

   ```bash
   pip install praw pydantic
   ```
3. Configure Reddit API credentials in the script (or use environment variables).
4. Run the notebook, modifying the `query` variable to search for relevant house price discussions in specific locations.

## Example Usage

Modify the query in the notebook to search for discussions in Manchester:

```python
query = "flat prices in Manchester"
search_results = search(query)
```

The search will return the top Reddit posts discussing flat prices in Manchester, along with user comments.

## Notes

Ensure you update the Reddit API credentials before running the notebook. The current credentials in the notebook are placeholders and should be replaced with your own.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
