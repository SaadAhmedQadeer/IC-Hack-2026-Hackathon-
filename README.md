# IC-Hack-2026-Hackathon-
IC Hack 26,  is the UK's Largest Student Run Hackathon! I participated in event and submit my AI Application. Sentinel Price vs Hype Stop reacting late. Sentinel Price vs Hype overlays AI news sentiment on stock charts. We quantify market mood to help you spot crashes or rallies before the price actually moves.

## What it does
Sentinel: Price vs Hype is a dashboard that acts as a "Lie Detector" for the stock market. It compares what a stock is doing (Price) against what people are feeling (Sentiment).

It Watches: The app pulls live stock prices (Reality) and scrapes the latest news headlines (The Hype).
It Reads: We use AI to read those headlines and give them a "Mood Score" from $-1.0$ (Panic) to $+1.0$ (Euphoria).
It Warns: The magic happens in the graph. We overlay these two distinct datasets. If the Sentiment (Red Line) drops off a cliff while the Price (Blue Line) is still high, the app screams "Divergence!"—giving you a heads-up that a crash might be coming.

## Working Prototype :
https://ic-hackathon-uk-2026-sentinel-price-vs-hype-msrwjuyrcsfrxhzgxd.streamlit.app/

## Built With
natural-language-processing
pandas
plotly
python
sentiment-analysis
streamlit
textblob
yfinance

## How we built it
We knew we only had 24 hours, so we chose a "Speed Stack" centered entirely on Python:

The Engine: We used Streamlit. It was a lifesaver, letting us turn our Python scripts into a beautiful web app in hours, not days.
The Data: We used yfinance to grab the hard numbers and simulated a news scraper to build our text corpus.
The Brains: We didn't overcomplicate the AI. We used TextBlob for NLP because it’s fast and lightweight, perfect for real-time "polarity scoring."
The Visuals: We used Plotly for the charts. We needed a "Dual-Axis" graph to make sense of the data (comparing a $180$ stock price to a $0.5$ sentiment score on the same screen).
## Challenges we ran into

The "Invisible Ink" Bug: Midway through, Streamlit’s default dark mode clashed with our custom buttons, making our text white-on-white. We had to hack some custom CSS to make the UI readable again.
The Demo Gods: We realized that relying on live web scraping during a 2-minute pitch is risky (bad WiFi, API bans). To save our demo, we engineered a robust "Demo Mode" that simulates realistic market data, ensuring our presentation is bulletproof.
Apples vs. Oranges: Plotting a stock price (like 200) next to a sentiment score (like 0.5) initially flattened the graph. We had to master Plotly’s secondary axes to make the correlation visually obvious.
## Accomplishments that we're proud of

Visualizing the Invisible: We successfully turned an abstract concept ("Market Sentiment") into a concrete line on a graph. Seeing the red line dip before the blue line is a genuine "Aha!" moment.
Zero to Hero: We went from an empty VS Code window to a live, deployed app on the cloud in under 24 hours.
$0 Budget: We built a powerful financial tool using 100% open-source libraries.
