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

Data was collected using the YouTube API to scrape comments from each of the selected videos. After retrieving the comments, preprocessing steps were applied, including:
- Removing emojis, special characters, and irrelevant text to clean the input data.
  
This ensured that the data was suitable for accurate sentiment analysis.

## Sentiment Analysis

The sentiment analysis was performed using Python libraries, including:
- **VADER** (Valence Aware Dictionary and sEntiment Reasoner) for sentiment scoring.
- **NLTK** for natural language processing and text preprocessing.
- **Pandas** for data handling and organization.

### Sentiment Classification:
- **Positive** (Scores > 0)
- **Neutral** (Scores = 0)
- **Negative** (Scores < 0)

## Aspect-Based Sentiment Analysis

To gain deeper insights, the comments were categorized into predefined *aspects*. These aspects helped understand which areas were most discussed and how viewers felt about them:

- **Product Design and Quality**: Comments related to the car's design, build quality, and features.
- **Brand Sentiment**: Comments focusing on the viewer's perception of the car brands.
- **Carwow**: Feedback about the content style and the platform itself.
- **Matt & Team**: Comments specifically referring to Matt Watson and his review team.

## BI Report Analysis

![Carwow - BI report](https://github.com/user-attachments/assets/40093b1e-a6df-4d8f-b973-d27f6e922f00)


A detailed Power BI dashboard was created to visualize the sentiment data and provide key insights for the Carwow team. Below is a summary of the insights from the report:

### Key Metrics:
1. **Total Sentiment Counts**: 
   - The **MG Cyberster** video had the highest number of sentimental comments (1,144), followed by the **Tesla Model 3** video (790 comments). The **Porsche 911** and **Bentley Continental GT** videos had fewer comments but still garnered significant attention.
   
2. **Sentiment for the Car Brands**:
   - **Tesla** and **Bentley** had the highest proportion of positive sentiment, with average sentiment scores of **0.50** and **0.48**, respectively. In contrast, **MG** and **Porsche** saw more negative sentiment, with average scores of **-0.45** and **-0.48**.

3. **Comments about Matt & Team**:
   - Feedback on **Matt & Team** was generally positive across all videos. The **Tesla Model 3** video had the highest positive sentiment (56.29%), while the **Bentley Continental GT** video had more negative feedback (61.33%).

4. **Sentiment on Product Design**:
   - The **Tesla Model 3** and **Bentley Continental GT** videos received the most praise for product design, with overwhelmingly positive comments. However, the **Porsche 911** and **MG Cyberster** videos attracted more critical remarks about their design.

5. **Channel Sentiment**:
   - The overall sentiment towards **Carwow** was positive, with strong appreciation for the content style. However, specific negative comments were made about certain car models and their design.

### Visualizations:

- **Sentiment Distribution**: Bar charts displaying the distribution of positive, negative, and neutral comments for each video.
  
    - [**New 782hp Continental GT!**]

      ![Carwow - Distribution GT](https://github.com/user-attachments/assets/26cafb3b-b308-4e62-8ff0-978b8b8b030e)



    - [**New MG Cyberster Review**]

       ![Carwow - Distribution MG](https://github.com/user-attachments/assets/36e24ad3-bb39-4578-868e-8be0d2976071)


    - [**Has Porsche Ruined the New 911?**] ![Carwow - Distribution Porsche](https://github.com/user-attachments/assets/1f88ca89-b1b1-4277-bb9f-93445a86e621)
    - [**NEW Tesla Model 3 Performance: 0-60mph & REVIEW**] ![Carwow - Distribution Tesla ](https://github.com/user-attachments/assets/e6bec275-9b44-4a3a-b36a-19d06291bd2a)

- **Aspect Sentiment**: Average sentiment for each aspect (Matt & Team, Product Design, Brand Sentiment, etc.), highlighting clear differences between positive and negative feedback.

  - [**New 782hp Continental GT!**]![Carwow - Aspect GT](https://github.com/user-attachments/assets/e4bc8164-7a90-4822-a50e-be11d56de0be)
  - [**New MG Cyberster Review**]![Carwow - Aspect MG](https://github.com/user-attachments/assets/564b72bf-d007-4eb7-9be9-a2fb776c59b5)
  - [**Has Porsche Ruined the New 911?**]![Carwow - Aspect Porsche](https://github.com/user-attachments/assets/f9dd8a7a-420a-4009-a5ca-c8e421468a54)
  - [**NEW Tesla Model 3 Performance: 0-60mph & REVIEW**]![Carwow - Aspect Tesla](https://github.com/user-attachments/assets/4d38d54f-d14d-4d3a-84d2-e861c1591202)

## Key Findings:

- The *Product Design and Quality* aspect received the most positive sentiment, especially for the **Tesla Model 3** and **Bentley Continental GT** videos.
- The *Brand Sentiment* aspect showed mixed reactions, with viewers showing concern on eletric car's
- Feedback on *Matt & Team* remained consistently positive across all videos, reflecting high viewer engagement and appreciation.
- The overall sentiment for **Carwow** was positive, though some negative feedback was tied to specific design elements in certain car models.

## Conclusion

This sentiment analysis provides valuable insights into audience reactions and perceptions of various car brands featured in Carwow's videos. The results can assist content creators, such as **Matt Watson**, and automotive brands in understanding how their content is received and adjusting their approach to better resonate with their audience. These insights are crucial for refining content strategy, addressing viewer concerns, and enhancing the overall viewer experience.

---

## **Note:**
This analysis is based solely on the comments provided by viewers under the videos and does not reflect opinions about the products themselves or the YouTube channel. The data was collected ethically using YouTube's publicly available API for research purposes only. No proprietary or sensitive data was used in this project, and the comments analyzed are publicly available to anyone viewing the videos.
