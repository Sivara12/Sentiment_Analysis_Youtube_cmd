# Sentiment Analysis Based on YouTube Comments

## Project Overview

This project aims to analyze the sentiment of YouTube comments on car review videos from *Carwow*, a popular platform known for its engaging automotive content, including car reviews, drag races, and performance comparisons. By performing sentiment analysis, we aim to uncover how viewers perceive the videos and identify key aspects of discussion.

### Videos Selected for Analysis:
1. **New MG Cyberster Review**
2. **Has Porsche Ruined the New 911?**
3. **NEW Tesla Model 3 Performance: 0-60mph & REVIEW**
4. **New 782hp Continental GT!**

### Objectives:
- Perform sentiment analysis on comments from each video to identify positive, negative, or neutral sentiments.
- Highlight key *aspects* that viewers focus on in their comments, such as *Product Design*, *Brand Sentiment*, *Carwow*, and *Matt & Team*.
- Provide insights into how different car brands and models are perceived by the audience.

## Data Collection

YouTube API was used to scrape comments from each of the videos. After retrieving the comments, the data was preprocessed by removing emojis, special characters, and unnecessary text to ensure clean inputs for sentiment analysis.

## Sentiment Analysis

The project uses a combination of Python libraries such as:
- `VADER` (Valence Aware Dictionary for Sentiment Reasoning) for sentiment scoring.
- `NLTK` for text preprocessing.
- `Pandas` for data handling and organization.
  
The sentiment scores were classified as:
- **Positive** (Scores > 0)
- **Neutral** (Scores = 0)
- **Negative** (Scores < 0)

## Aspect-Based Analysis

In addition to the overall sentiment, we grouped comments into predefined *aspects* to understand which parts of the video people talked about the most and their corresponding sentiments. The aspects include:
- **Product Design and Quality**: Comments related to car design, build, and features.
- **Brand Sentiment**: Comments regarding the overall perception of the car brand.
- **Carwow**: Feedback about the Carwow team and the content style.
- **Matt & Team**: Comments specifically mentioning Matt Watson and the review team.

## Results and Visualizations

The following visualizations were generated:
- **Sentiment Distribution**: A breakdown of positive, neutral, and negative comments for each video.
- **Aspect Sentiment**: Visualizing the average sentiment score per aspect to show which areas viewers felt most positively or negatively about.

Key Findings:
- The *Product Design and Quality* aspect generally had the highest positive sentiment, especially for the Tesla Model 3 and Continental GT videos.
- There was a mixed response in the *Brand Sentiment* aspect, with viewers showing concern in videos like "Has Porsche Ruined the New 911?"
- Feedback on *Matt & Team* remained largely positive across all videos.

## Conclusion

This project highlights the importance of sentiment analysis in understanding audience reactions to content. The insights from this analysis could help content creators and car brands alike to tailor their messaging and product features based on viewer sentiment.
