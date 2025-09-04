# MTG Standard Meta Analysis: Top 20 Decks (Last 90 Days) 🎴

## Overview
This project analyzes the top 20 performing Magic: The Gathering (MTG) Standard decks over the last 90 days (June–August 2025) to identify metagame trends, dominant cards, and powerful card combinations. By scraping decklists and performance data from mtgdecks.net and aetherhub.com, the project provides insights into the Standard format's competitive landscape, highlighting potential problem cards or combos for players and deck builders.

## Objectives
- Identify the top 20 Standard decks based on winrates and tournament performance.
- Analyze decklists to detect frequently used cards and synergies.
- Visualize metagame trends and card prevalence to uncover dominant strategies.
- Provide actionable insights for MTG players and deck builders.

## Data Sources
- **mtgdecks.net**: Provides decklists, winrates, and tournament results for Standard format (over 12,739 matches from March–August 2025).
- **aetherhub.com**: Offers archetype winrates (e.g., UR Soul Cauldron at 36.92%) and detailed decklists from recent tournaments.
- **Scryfall API** (optional): Used to validate card names and fetch card attributes (e.g., mana cost, type).

## Methodology
1. **Data Collection**: Scraped decklists and performance data using Python (`requests`, `BeautifulSoup`, `selenium` for dynamic content).
   - Targeted `<td class="sort">` containers with `<strong name="...">` tags for deck names.
   - Extracted winrates and decklists from associated tables or sections.
2. **Data Cleaning**: Standardized card names, removed duplicates, and handled missing winrates using pandas.
3. **Analysis**: 
   - Ranked decks by winrate to identify the top 20.
   - Counted card frequencies across decklists to detect trends.
   - Analyzed card combinations for potential synergies or problem combos.
4. **Visualization**: Created bar charts, heatmaps, and time-series plots using Matplotlib and Seaborn to show archetype prevalence and card trends.

## Results
- **Top Decks**: Identified archetypes like UR Soul Cauldron (36.92% winrate) and Dimir Aggro (20.00%) as top performers.
- **Key Cards**: Highlighted frequently used cards (e.g., [insert example cards]) driving metagame trends.
- **Combos**: Detected potential problem combos (e.g., [insert example combo]) based on card co-occurrence.
- **Visuals**: Generated charts showing archetype winrates and card frequencies over the 90-day period.

*Note*: Detailed results and visualizations are in the `output/` folder.

## Project Structure