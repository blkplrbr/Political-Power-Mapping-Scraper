# Political Power Mapping & Network Analysis Engine

## Project Overview
Developed an open-source intelligence (OSINT) data pipeline designed to map the "Winning Coalition" (selectorate) of local politicians. By scraping campaign finance records, committee assignments, and public endorsements, this tool generates a network graph that reveals the interconnected relationships between politicians, corporate donors, and political action committees (PACs).

## The Problem
Grassroots political organizations often lack the data infrastructure to understand who truly holds power in their districts. Pitching progressive policies is difficult when you don't know which corporate donors are bankrolling the opposition. This tool automates the opposition research process, allowing organizers to identify the weakest links in a politician's support network.

## Technical Stack
*   **Language:** Python
*   **Libraries:** BeautifulSoup (Web Scraping), Pandas (Data Structuring), NetworkX (Graph Building)
*   **Visualization:** Gephi or Power BI (Network Mapping)
*   **Data Sources:** State Board of Elections (Campaign Finance), Legislative Rosters (Committee Assignments), Local News Archives.

## Methodology (The Pipeline)
1.  **Data Extraction:** Scrape state campaign finance databases to pull donor names, amounts, and dates. Scrape legislative rosters to pull committee assignments and voting records.
2.  **Entity Resolution:** Clean and standardize names across datasets (e.g., ensuring "Smith, John" and "John Smith" are merged).
3.  **Network Graph Construction:** Use Python's `NetworkX` library to create nodes (politicians, donors, PACs) and edges (financial transactions, endorsements, committee memberships).
4.  **Analysis:** Calculate the centrality of each node to identify the "Kingmakers" (the donors connected to the most politicians).

## Business/Organizing Impact
*   Replaces expensive, proprietary political data tools with a free, open-source pipeline.
*   Provides local organizers with a visual map of their political terrain.
*   Enables targeted campaigns against specific corporate interests rather than broad, unfocused protests.

## Status
🚧 **Work in Progress:** The BeautifulSoup scrapers and NetworkX scripts are currently under development.
