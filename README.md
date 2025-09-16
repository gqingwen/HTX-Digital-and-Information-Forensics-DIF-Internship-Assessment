# HTX-Digital-and-Information-Forensics-DIF-Internship-Assessment
My Submission for the take-home assessment

# About
This repository contains the Jupyter Notebook containing my submission, and screenshots of results and diagrams

# Project Overview
For the take-home assessement, I attempted Challenge 2: Data Science (Cryptocurrency) Assessment. No additional installation or set-up is required, just download the Jupyter Notebook and run all the cells within

# Challenge Overview
Write a Python script(s) or Jupyter Notebook(s) that:
Fetches historical cryptocurrency data
Performs simple analysis
Output key insights/metrics
 
---

# Task 1
Use a public blockchain API (e.g. Etherscan or Blockchain.com) to:
Query recent transactions of a crypto wallet address (of your choice)
Plot a simple graph:
Nodes = Wallet addresses
Edges = Transactions
Focus on a small subset (e.g. 10–20 transactions) for clarity
(Bonus) Provide insights on the activity / detection of possible illicit activity

For this, I made use of the Etherscan API to gather data of the 15 latest transactions from the crypto wallet address of BuilderNet.
I then plotted a graph with the nodes being the wallet addresses and edges being the transactions.
Each transaction consisted of the BuilderNet wallet sending etherium to other wallets, as shown by the direction of the arrow.
The value of each transaction is labelled on the arrow's themselves.
The graph takes into account multiple transactions between the same pairs of senders and receivers, and these transactions are displayed accordingly

The main insights that I drew was mainly about some of the transactions taking place on the same day and same time, down to even having multiple transactions in the same second.
This showed me that these transactions are likely automated to take place when some condition is met, instead of being done by a human being.
This alone is insufficient to prove that illicit activity is taking place.

# Task 2
Perform basic forensics analysis:
Select a crypto token of your choice where there is a time period (e.g. 7-day or 30-day) with possible
unusual market activity / illicit activity (e.g. pump and dump) involved
Highlight movements that are potential red flags
Results can be in the form of:
Time series with highlighted anomalies (e.g. volume spikes) and/or;
Histograms of transaction sizes or times and/or;
Wallet-level heatmaps and/or;
Annotated charts with labels like “suspicious activity detected”

For this, I choose the Libra token and again, made use of the Etherscan API to explore the transactions of the token.
I explored the transaction data year by year, and for 2021 I discovered something interesting.
In January of that year, on the 25th of Jan in particular, there was an exceptionally high amount of transactions and total transaction value as compared to the rest of the year.
That was highky suspicious and is likely a sign of illicit activity such as pump and dump activities
I then plotted 2 bar charts and a histogram to visualise this event.



# References
- https://docs.etherscan.io/
- https://stackoverflow.com/questions/22785849/drawing-multiple-edges-between-two-nodes-with-networkx
- https://networkx.org/documentation/stable/tutorial.html

# Mini-Reflection
Regardless of the outcome, attempting this take home assessment gave me the opportunity to learn quite a bit about cryptocurrency transactions and how to query public blockchain apis, which I enjoyed learning and figuring out how to do.
