# SEC-Filing-Similarity-Indexing-for-Trading-Signals
This project aims to compare SEC filings of given years with the previous years to check for similarity in language and usage of words among eight large-cap technology companies as a potential trading signal for positive market returns.
The hypothesis posits that a lower similarity score may indicate a positive return, uncorrelated with general market returns. The analysis spans from 2018 to 2022, excluding 2023 due to incomplete filings, and focuses on the following companies:

Apple
Microsoft
Google
IBM
AMD
Meta (formerly Facebook)
Amazon
Netflix
Market return proxies are obtained from a benchmark ETF, with analysis conducted over 1-week and 4-week windows post-filing to capture the immediate market response.

Getting Started
Dependencies
Wolfram Mathematica 13.3 or later for computational analysis.
Internet access for SEC filings retrieval.
Installation
Ensure Wolfram Mathematica is properly installed on your system. Clone this repository to your local machine and ensure you have a stable internet connection to fetch SEC filings.

Data Source
SEC filings URLs are programmatically accessed. Ensure the URLs are up to date for each company involved in the analysis.

Key Functions and Analysis
Word Extraction from Filings
A function myHelperFunctionFilling extracts all words from the given URL of the company's filings and creates an array of words for analysis.

Similarity Score Calculation
jaccardSimilarity calculates the Jaccard similarity score between two arrays of words from consecutive years' filings, aiding in identifying changes in language and terminology.

Market Analysis
plotCumFracChg plots the cumulative fractional change of securities and the difference between the security's and the benchmark ETF's returns to evaluate the investment signal.

Analysis Execution
For each company, execute the word extraction and similarity score calculation for the specified years. Then, conduct the market analysis using the determined windows post-filing.

Results Interpretation
The analysis includes plotting similarity scores over time and comparing these with market performance. Lower similarity scores are hypothesized to correlate with positive, market-independent returns.

Authors
Krish
License
This project is licensed under the MIT License - see the LICENSE.md file for details.

Acknowledgments
Inspiration from financial market analysis theories.
Working with my wonderful team consisting Nikhil, Rushali, Tejaswi and Subham
Wolfram Research for Mathematica software.
