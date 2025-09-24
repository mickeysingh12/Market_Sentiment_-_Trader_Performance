# Market Sentiment & Trader Performance

## Overview

This project investigates the relationship between **market sentiment**
(using the Fear & Greed Index) and **trader performance**. The goal is
to explore whether emotional market sentiment aligns with or influences
trading outcomes, potentially providing insights into better
decision-making.

------------------------------------------------------------------------

## Project Structure

    Market_Sentiment_&_Trader_Performance/
    ├── data/
    │   ├── fear_greed_index.csv      # Fear & Greed Index data (market sentiment)
    │   ├── historical_data.csv       # Historical trader performance data
    ├── notebooks/
    │   ├── Market_Sentiment_&_Trader_Performance.ipynb  # Jupyter notebook with data preparation and analysis
    ├── visuals/
    │   ├── timeline_chart.png        # Visual comparing dataset timelines
    ├── README.md                    # Project overview
    └── requirements.txt             # Python dependencies

------------------------------------------------------------------------

## Requirements

The following Python libraries are required to run this project:

-   pandas
-   numpy
-   matplotlib
-   reportlab
-   pptx

You can install the necessary dependencies by running:

    pip install -r requirements.txt

------------------------------------------------------------------------

## Getting Started

### 1. **Clone the repository**:

``` bash
git clone https://github.com/mickeysingh12/Market_Sentiment_Trader_Performance.git
```

### 2. **Data Preparation**:

The data files (`fear_greed_index.csv` and `historical_data.csv`) must
be loaded into the `data/` directory.

The Jupyter notebook (`Market_Sentiment_&_Trader_Performance.ipynb`)
will walk through the following steps: - **Cleaning and formatting** the
timestamp columns. - **Merging** the data on the `date` column to align
market sentiment and trader performance. - **Analyzing** the
relationship between the two datasets.

### 3. **Run the Jupyter Notebook**:

Open the notebook and run the code cells sequentially to: - Process the
data. - Investigate the issues with merging datasets (due to
non-overlapping dates). - Generate insights once data alignment is
fixed.

### 4. **Generate Reports**:

After running the notebook, you can generate a **PDF report** and
**PowerPoint slides** for presentation and documentation purposes. The
reports will summarize the project and include visuals of the dataset
comparison.

------------------------------------------------------------------------

## Challenges

1.  **Timestamp Conversion**:
    -   The `Timestamp` column in the historical data did not convert
        properly to datetime objects, leading to `NaT` values and no
        matching dates for merging.
2.  **Date Mismatch**:
    -   Even after cleaning, no overlap was found between the two
        datasets, which requires further alignment of the date ranges.

------------------------------------------------------------------------

## Next Steps

1.  **Fix Timestamp Parsing**:
    -   Investigate the format of the `Timestamp` column in historical
        data and apply correct conversion methods.
2.  **Align Date Ranges**:
    -   Ensure that both datasets cover the same time period before
        attempting to merge again.
3.  **Analysis**:
    -   Once the datasets are aligned, analyze the correlation between
        sentiment and trader performance using statistical methods.

------------------------------------------------------------------------

## Contributing

Feel free to fork the repository and make improvements. If you have any
suggestions or find bugs, please open an issue or submit a pull request.

------------------------------------------------------------------------

