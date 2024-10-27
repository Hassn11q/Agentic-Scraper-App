# Agentic Scraper 🕷️

Agentic Scraper is a web scraper designed to extract product information from websites using AgentQL and Playwright, storing the results in CSV and JSON formats for easy data analysis.


## Features

- **Field Selection**: Allows users to select specific fields to scrape (e.g., product name, price, number of reviews, and rating).
- **Pagination Handling**: Automatically scrapes multiple pages of results.
- **Customizable GraphQL Queries**: Users can adjust queries based on desired data fields.
- **Streamlit UI**: User-friendly interface for configuring scraping settings.
- **Data Download Options**: Export scraped data to CSV and JSON formats.


## Prerequisites

Before you begin, ensure you have the following:

- Python 3.9+
- [Playwright](https://playwright.dev/) for browser automation
- AgentQL account and API key from the [AgentQL Dashboard](https://dev.agentql.com/api-keys)

## Installation

1. Clone this repository:
   ```
   https://github.com/Hassn11q/Agentic-Scraper.git
   cd Agentic-Scraper
   ```

2. Install the required Python packages:
   ```
   pip install -r requirements.txt
   ```

3. Install Playwright browsers:
   ```
   playwright install
   ```

4. Get your AgentQL API key from [AgentQL Dashboard](https://dev.agentql.com/api-keys)

5. Create a `.env` file in the project root and add your AgentQL API key:
   ```
   AGENTQL_API_KEY=your_api_key_here
   ```

## Usage

1. **Start the Streamlit App**:
   ```bash
   streamlit run app.py


2. **Configure Scraper Settings**:
- Enter the target URL.
- Use the Field Selection toggle in the sidebar to add desired fields.
- Set pagination options to specify the number of pages to scrape.

3. **Run the Scraper**:
- Click the Scrape button in the sidebar to initiate scraping.
- The scraping progress and data extraction details are displayed in the main area.

4. **Download the Results**:
Once the scraping is complete, download the data as a CSV or JSON file.

  
## Configuration

You can customize the following variables in app.py to adjust the scraper's behavior:

- `url_input`: Target URL for the e-commerce website.
- `items_query`: GraphQL query to fetch specific product data fields.
- `pagination_query`: GraphQL query for pagination.

## Example Queries
- `Product Query`: Customize the fields in items_query based on the available product attributes.
- `Pagination Query`: Use pagination_query to check pagination status and handle multi-page scraping.

## Acknowledgments

- [AgentQL](https://dev.agentql.com/) for providing the querying capabilities
- [Playwright](https://playwright.dev/) for browser automation Agentic-Scraper
