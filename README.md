# Project01_TDS
- Data was scraped from the GitHub API, focusing on Zurich users with over 50 followers and their repositories.
- The most surprising insight was that BitBake, though relatively obscure, had the highest average stars per repository.
- Developers should prioritize Python and JavaScript in Zurich, as they are popular among recent and top-followed users.

## Project Overview

This project collects GitHub user data from Zurich with over 50 followers, including detailed information about users and their repositories. The data has been processed and stored in two CSV files, `users.csv` and `repositories.csv`, formatted to preserve the integrity of the GitHub API response data.

## Files Included

- **users.csv**: Contains information about users from Zurich with fields like `login`, `name`, `company`, `location`, and more.
- **repositories.csv**: Lists repositories for each user, detailing `full_name`, `created_at`, `stargazers_count`, `language`, and other repository-specific fields.
- **Code**: The scraping and data processing code is included to allow reproducibility of the dataset.
  
## Data Analysis Insights

The data analysis yielded the following insights:

1. **Followers and Repository Count Correlation**: The correlation between followers and the number of public repositories is low (0.065), suggesting that simply creating more repositories does not strongly correlate with more followers.
   
2. **Most Popular License and Language**: The MIT License was the most common among Zurich developers, and Python was the most frequently used language. JavaScript also emerged as a popular choice for users who joined post-2020.
   
3. **Developer Strength**: Calculated as `leader_strength`, users with a high follower-to-following ratio include riscv, bpasero, and Seldaek, indicating influential users who follow fewer people.
   
4. **Project and Wiki Enabling Correlation**: The correlation between projects and wiki-enabled repositories was negligible, indicating no significant trend in enabling both features together.

## Recommendations for Developers

1. **Focus on Popular Languages**: Python and JavaScript are strong choices for Zurich developers; maintaining proficiency in these languages may enhance visibility.
2. **Engage with Follower Influencers**: Networking with high `leader_strength` developers could be strategic, given their influence.
3. **License Visibility**: Using well-known licenses, like MIT, may increase trust and engagement with repositories.
