# Sentiment Analysis Based on YouTube Comments

## Project Overview

This project focuses on analyzing the sentiment of YouTube comments on car review videos from *Carwow*, a popular platform known for its engaging automotive content, including car reviews, drag races, and performance comparisons. By performing sentiment analysis, the aim is to uncover how viewers perceive these videos and identify key aspects of the discussion.

### Videos Selected for Analysis:
1. [**New MG Cyberster Review**](https://www.youtube.com/watch?v=olcjaZYaUvY)
2. [**Has Porsche Ruined the New 911?**](https://www.youtube.com/watch?v=-2_zFZgE5Lo)
3. [**NEW Tesla Model 3 Performance: 0-60mph & REVIEW**](https://www.youtube.com/watch?v=mmjN3Z4HcEI)
4. [**New 782hp Continental GT!**](https://www.youtube.com/watch?v=UMIld6-lIQ8)

### Objectives:
- Perform sentiment analysis on comments from each video to classify them as positive, negative, or neutral.
- Highlight key *aspects* that viewers focus on in their comments, such as:
  - **Product Design and Quality**
  - **Brand Sentiment**
  - **Carwow** (feedback on the platform and the videos)
  - **Matt & Team** (comments about the host and the review team)
- Provide insights into how different car brands and models are perceived by the audience.

## Data Collection

Data was collected using the YouTube API to scrape comments from each of the selected videos. After retrieving the comments, preprocessing steps were applied, such as:
- Removing emojis, special characters, and irrelevant text for clean input.
  
This step ensured that the data was suitable for accurate sentiment analysis.

## Sentiment Analysis

The sentiment analysis was performed using several Python libraries, including:
- **VADER** (Valence Aware Dictionary and sEntiment Reasoner) for sentiment scoring.
- **NLTK** for natural language processing and text preprocessing.
- **Pandas** for data handling and organization.

### Sentiment Classification:
- **Positive** (Scores > 0)
- **Neutral** (Scores = 0)
- **Negative** (Scores < 0)

## Aspect-Based Sentiment Analysis

To gain deeper insights, the comments were categorized into predefined *aspects*. These aspects helped to understand which areas were most discussed and how viewers felt about them:

- **Product Design and Quality**: Comments related to the car's design, build quality, and features.
- **Brand Sentiment**: Comments focusing on the viewer's perception of the car brands.
- **Carwow**: Feedback about the content style and the platform itself.
- **Matt & Team**: Comments specifically referring to Matt Watson and his review team.

## BI Report Analysis

![BI report](https://github.com/user-attachments/assets/b2cb3493-6ab7-40d9-b617-c54cdbfc402a)

A detailed Power BI dashboard was created to visualize the sentiment data and provide key insights for the Carwow team. Below is a summary of the insights from the report:

### Key Metrics:
1. **Total Sentiment Counts**: 
   - The analysis revealed that the **MG Cyberster** video had the highest number of comments (1,144), followed by **Tesla Model 3** (790 comments). The **Porsche 911** and **Bentley Continental GT** had fewer comments but still garnered significant attention.
   
2. **Sentiment for the Car Brands**:
   - **Tesla** and **Bentley** had the highest proportion of positive sentiment, with an average sentiment score of **0.50** and **0.48**, respectively. In contrast, **MG** and **Porsche** saw a more negative average sentiment, with **-0.45** and **-0.48** scores.

3. **Comments about Matt & Team**:
   - The feedback on **Matt & Team** remained mostly positive across all videos. The **Tesla Model 3** video had the highest positive sentiment (56.29%), while the **Bentley** video had the highest negative feedback (61.33%). 
   
4. **Sentiment on Product Design**:
   - The analysis highlighted that **Tesla Model 3** and **Bentley** were praised for their product design, receiving the most positive sentiment. However, **Porsche 911** and **MG Cyberster** saw more critical comments regarding their design.
   
5. **Channel Sentiment**:
   - The overall sentiment for **Carwow** as a platform was positive, with a strong appreciation for the content style, though certain negative comments surfaced regarding specific car models and design elements.

### Visualizations:
- **Sentiment Distribution**: Bar charts showing the distribution of positive, negative, and neutral comments for each video.
   [**New 782hp Continental GT!**]![Carwow - Distribution GT](https://github.com/user-attachments/assets/26cafb3b-b308-4e62-8ff0-978b8b8b030e)
   [**New MG Cyberster Review**]![Carwow - Distribution MG](https://github.com/user-attachments/assets/36e24ad3-bb39-4578-868e-8be0d2976071)
   [**Has Porsche Ruined the New 911?**]![Carwow - Distribution Porsche](https://github.com/user-attachments/assets/1f88ca89-b1b1-4277-bb9f-93445a86e621)
   [**NEW Tesla Model 3 Performance: 0-60mph & REVIEW**] ![Carwow - Distribution Tesla ](https://github.com/user-attachments/assets/e6bec275-9b44-4a3a-b36a-19d06291bd2a)

  
- **Aspect Sentiment**: Average sentiment for each aspect (Matt & Team, Product Design, Brand Sentiment, etc.) with clear visual differentiation between positive and negative feedback.
- **Sentiment Trends by Video**: A breakdown of the sentiment trends for each individual video.

## Conclusion

This project demonstrates how sentiment analysis can provide valuable insights into audience reactions. The findings can help content creators like **Matt Watson** and car brands understand how viewers perceive their videos and adjust their messaging accordingly. These insights are particularly useful for improving content strategy, addressing viewer concerns, and enhancing the overall viewing experience for Carwow's audience.

---

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
