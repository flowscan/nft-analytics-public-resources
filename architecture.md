# Architecture

The project can be divided into four major parts. 
- The marketplace indexers
- Metrics aggregator
- GraphQL API
- Web Front-end

![architecture](https://user-images.githubusercontent.com/16462328/148936955-27750a3a-f075-4402-bcd3-2abfab3aca93.png)

## Marketplace Indexers
A service that extracts and indexes marketplace events (listings and sales). This service can source its data from Flowscan's internal indexed events feed. This service need to combine sales and listings from different marketplaces and stores it in one unified database.

Additionally, this service need to keep a state of NFT prices based on its latest sales.

## Metrics Aggregator
This service aggregates data from the indexed marketplace sales and Flowscan API (to get NFT holders, list of NFTs out there, etc) to create and store time-series analytics data.

Time-series data including:
- NFT price floor and average from the marketplace sales
- Number of holders
- Number of tokens listed on the marketplace
- Sales activity (e.g. number of sales / day)
- More metrics could be requested by the *Frontend* team

## GraphQL API
Expand the current Flowscan's GraphQL API to includes queries for
- Marketplace listings and sales
- Historical NFT listings and sales
- Metrics made by the *Metrics Aggregator* team 
- Other queries requested by the *Frontend* team

## Web Frontend
Design and develop the front-end web interface for

### NFT Projects Analytics 
Each NFT projects on Flow would have an analytics / stats page for them. It will be located as a tab below the contract info for the NFT contract. 

For example, for TopShot in https://flowscan.org/contract/A.0b2a3299cc857e29.TopShot with a new tab called "Analytics". 

### Global NFT stats page

Located at https://flowscan.org/nft-stats. 

- Show the volume statistics for the marketplaces on Flow
- Display a table of NFT projects on Flow with their respective volume 