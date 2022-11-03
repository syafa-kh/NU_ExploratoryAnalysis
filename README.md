# Dataset Overview
This is a translated Chinese webnovel data scraped from NovelUpdates on October 2022. There are 11 columns detailing the novel and its performance:
- title           : Novel's title
- description     : Novel's summary/description in English
- genres          : List of genres associated with each novel
- tags            : List of tags used to describe each novel's content
- overall_rates   : Novel's rating ((number of stars * star votes)/total voters)
- \*\_star_votes  : Number of voters who rate each novel with * stars
- rec_list        : Other novels recommended by readers of each novel

# Main Goal
Performing exploratory data analysis to understand the data for further machine learning process while simultaneously drawing insights regarding most popular novels and their performance

# Main Questions
1. Which type of novels are the most popular? Which genres and tags?
2. How does each genre and tag performs? Which ones have the highest performance?
3. How does each genre and tag correlate to another?

# Answers Based On Exploration
1. Romance is the most translated genre on the site, reflected by 'handsome male lead' as the most used tag. However, the most popular novel with the highest total voters is a stallion novel called Against The God
2. Romance placed 5th in average rating and has 5th highest 5-star voters amongst other top genres. The first positions in both categories are occupied by yaoi, a genre with gay main characters. Meanwhile, 'Devoted Love Interest' is the tag with highest average rating
3. Romance is a genre made up of light-read books which has high correlation to other light-read genres like slice of life or drama. There are also interesting connection between NSFW Genres and Genres Targeted Towards Men, Sexuality Related Genre and Others, and Genres and Performance. 

# Future Recommendations
Is there any visible pattern for rec_list? Is it possible to build a graph on how they're all related? Can we see clusters of novels or genres?
(Tried using NetworkX to get the graph and visualize it both using plotly and PyVis but didn't work out very well)