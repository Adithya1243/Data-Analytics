# YouTube Channel Analysis: Pewdiepie and MrBeast

## 1. Introduction

This project involves scraping and analyzing video metadata from two popular YouTube channels, Pewdiepie and MrBeast, to understand viewing trends over the years. The aim is to assess how factors like view count, like count, and video duration influence video popularity, culminating in a machine learning model predicting new video popularity.

## 2. Data Collection

Data was collected using the YouTube Data API v3 from a Google Cloud account. The project utilized publicly available data, with deeper insights from YouTube Analytics API remaining inaccessible as it's limited to channel owners.

## 3. Data Wrangling

The process involved:
- Merging data from two CSV files into a single DataFrame.
- Converting 'publishedAt' from string format to datetime for ease of analysis.
- Scaling down view counts for simplicity.
- Converting video duration from ISO 8601 format to minutes.
- Splitting video tags into individual elements for detailed analysis.

Libraries used: pandas, isodate, matplotlib.pyplot, seaborn.

## 4. Data Visualization

Visualizations were created to address the research questions, focusing on yearly trends, correlation between likes and views, top tags in videos, average likes vs. video duration, and average duration in relation to popularity metrics.

## 5. Data Analysis

A Random Forest model was developed to predict video views based on duration, likes, and comment count. The model's performance was evaluated using Mean Squared Error (MSE), which stood at 206.62.

## 6. Conclusion

Key findings include:
- Shorter videos from PewDiePie and MrBeast tend to be more popular.
- Tags like 'unboxing' and 'iPhone' are highly popular.
- Likes and comments are strong indicators of video popularity.

## Future Improvements

Future project enhancements could include:
- Accessing demographic details via YouTube Analytics API.
- Focusing on specific video categories for targeted user behavior analysis.
- Incorporating sentiment analysis of comments, especially since the dislike count is no longer available.

## Column Descriptions

- `videoId`: Unique video ID
- `title`: Video title
- `publishedAt`: Upload date
- `categoryId`: Numerical video category ID
- `categoryName`: Video category name
- `tags`: Associated video tags
- `viewCount`: Total views
- `likeCount`: Total likes
- `dislikeCount`: Dislike count (not available due to policy update)
- `commentCount`: Total comments
- `duration`: Video duration
- `subscriberCount`: Channel subscriber count

## Research Questions Explored

- Yearly trends in video views.
- Correlation between like count and view count.
- Top 10 tags in videos.
- Relationship between average likes and video duration.
- Average video duration's impact on popularity.
