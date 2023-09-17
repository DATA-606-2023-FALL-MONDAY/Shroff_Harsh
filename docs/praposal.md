# Project Proposal
 
## 1. Title and Author

- **Project Title:** AirbnbLens - Capturing Your Style
- **Prepared for** UMBC Data Science Master Degree Capstone by Dr Chaojie (Jay) Wang
- **Author Name:** Harsh Shroff 
<!-- - Link to the author's GitHub profile
- Link to the author's LinkedIn progile
- Link to your PowerPoint presentation file
- Link to your YouTube video  -->
    
## 2. Background

### What is it about?

The topic is about the development of an Airbnb Photo-Based Recommendation System. This system aims to provide Airbnb users with personalized recommendations for accommodations based on the photos of their previous stays. It utilizes computer vision and machine learning techniques to analyze images and match them with similar Airbnb listings. The system benefits both travelers looking for unique and stylish accommodations and hosts seeking insights into their competition.

### Why does it matter?

The project matters for several reasons:

- **Enhanced User Experience:** Airbnb travelers often seek accommodations that align with their aesthetic preferences and style. This system enhances their experience by offering tailored recommendations based on their past experiences.

- **Competitive Advantage for Hosts:** Airbnb hosts can gain a competitive edge by understanding what makes their listing unique or similar to others in the area. This knowledge allows hosts to make data-driven decisions to improve their offerings.

- **Data-Driven Travel:** As the travel industry increasingly relies on data-driven decision-making, this project contributes to the trend by providing travelers with a more data-rich and personalized approach to selecting accommodations.

### What are your research questions?

The research questions for this project may include:

1. Can computer vision and image analysis techniques accurately assess the style and aesthetics of Airbnb accommodations based on user-provided photos?

2. How can machine learning algorithms be leveraged to recommend Airbnb listings that match a user's style preferences?

3. What additional features and data can enhance the accuracy and personalization of recommendations?

4. How can this system benefit both Airbnb travelers and hosts, and what metrics can be used to measure its impact?

## 3. Data

### Data Sources

The primary data source for this project is the InsideAirbnb dataset, which is published by Airbnb and contains comprehensive information about Airbnb listings worldwide, including property details, host information, and photos.

### Data Size

The size of the dataset may vary over time as new listings are added and existing ones are updated. As of the latest update, the dataset could be several gigabytes in size due to the inclusion of photos.

### Data Shape

The dataset typically consists of thousands to millions of rows and multiple columns, depending on the geographical coverage and the number of listings. Each row represents a unique Airbnb listing.

### Time Period

The data may not be strictly time-bound, but it covers listings available at the time of data collection. The dataset can include listings from different years, and it is essential to consider the publication date of each listing.

### What does each row represent?

Each row in the dataset represents a unique Airbnb listing, including information about the property, host, location, pricing, and, importantly, photos associated with that listing.

### Data Dictionary

A sample data dictionary might include the following information:

- **Columns Name:** These could include columns such as "listing_id," "property_type," "room_type," "accommodates," "bedrooms," "bathrooms," "host_id," "neighborhood," "price," and "photo_urls."

- **Data Type:** Data types may include integers, floats, strings, dates, and images (for photo URLs).

- **Definition:** Definitions would describe the meaning of each column, e.g., "listing_id" represents the unique identifier of an Airbnb listing.

- **Potential Values:** For categorical variables like "property_type" or "room_type," potential values might include "Apartment," "House," "Private room," "Entire home/apt," etc.

### Target/Label Variable for ML Model

The target variable for the machine learning model in this project would likely be a binary classification label indicating whether a particular Airbnb listing is a good match for the user's style preferences based on their provided photos.

### Features/Predictors for ML Models

Potential features or predictors for the machine learning model could include attributes such as "property_type," "room_type," "bedrooms," "bathrooms," "neighborhood," and the results of image analysis (e.g., style, color palette, sentiment) from the provided photos.

The data and data dictionary will be crucial in building and training machine learning models and in conducting analyses to answer the research questions and create a functional recommendation system.
