
---

# Reddit Real Estate Agent using Gemma2:9b

This project aims to provide a recommendation system using data scraped from Reddit, specifically related to house prices in the United Kingdom. It employs the Gemma2:9b language model for natural language responses and filtering relevant Reddit posts based on user queries.

## Project Overview

The notebook implements a system that:
1. Scrapes Reddit for housing-related posts using the `praw` library.
2. Filters results to focus on specific keywords related to real estate, apartment prices, and house prices.
3. Extracts the most relevant comments from the top posts and summarizes the findings.
4. Uses the **Gemma2:9b** language model to provide concise natural language responses to user queries.

## Features

- **Reddit Scraping**: Utilizes the `praw` library to fetch posts from relevant subreddits like `HousingUK`.
- **Natural Language Processing**: Uses the Gemma2:9b model to generate user-friendly answers based on the Reddit posts.
- **Comment Filtering**: Extracts the top comments with a minimum of 20 upvotes and provides them as part of the recommendation.
- **Data Output**: Provides recommendations in a human-readable format, including average prices and a summary of housing trends.

## Prerequisites

- Python 3.12 or higher
- Required Python libraries:
  - `praw`
  - `pydantic`
  - `Gemma2` language model
  - `datetime`

You will also need access to Reddit's API to retrieve the data.

## Setup

1. Install the required packages:
   ```bash
   pip install praw pydantic
   ```

2. Ensure you have a valid Reddit API key, which can be obtained from [Reddit's Developer Tools](https://www.reddit.com/prefs/apps).

3. Run the notebook to collect and process Reddit posts related to UK housing prices.

## Usage

1. Modify the query variable in the notebook to search for real estate data in your desired location, for example:
   ```python
   query = "flat prices in Manchester"
   ```

2. Execute the notebook to generate housing recommendations based on the most upvoted Reddit posts. The notebook will return a summarized view of the housing market in the region specified.

3. Use the `final_answer` function to format the output in a user-friendly format.

## Model Information

The **Gemma2:9b** model used in this project is small but still offers impressive performance. It's a great choice for local execution, providing relevant and accurate responses in real-time without needing extensive cloud infrastructure.

---