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

The primary data source for this project is the [InsideAirbnb](http://insideairbnb.com/get-the-data/) dataset, which is published by Airbnb and contains comprehensive information about Airbnb listings worldwide, including property details, host information, and photos.

### Data Size

I have shortlisted 8 cities from the East Coast of the USA namely Asheville, North Carolina, Boston, Massachusetts, Cambridge, Massachusetts, Jersey City, New Jersey, New York City, New York, Newark, New Jersey, Rhode Island, Rhode Island.

Combining altogether, 
- the *CSV* files are about 160 MBs in size.
- the size of *images* folder is ~6.5 GBs (if taken 1 image per listing).


### Data Shape

There are 75 columns and 62330 rows in the dataset.

### Time Period

The data is not strictly time-bound, but it covers listings available at the time of data collection. The dataset include listings from different years, and it is essential to consider the publication date of each listing.

### What does each row represent?

Each row in the dataset represents a unique Airbnb listing, including information about the property, host, location, pricing, and, importantly, photos associated with that listing.

### Data Dictionary

A sample data dictionary might include the following information:

- **Columns Name:** These could include columns such as `listing_id, property_type, room_type, accommodates, bedrooms, bathrooms, host_id, neighborhood, price, latitude, longitude,` and `photo_urls.`

- **Data Type:** Data types are include integers, floats, strings, dates, and images (for photo URLs).

- **Potential Values:** For categorical variables like "property_type" or "room_type," potential values might include "Apartment," "House," "Private room," "Entire home/apt," etc.

### Target/Label Variable for ML Model

A binary classification label indicating whether a particular Airbnb listing is a good match for the user's style preferences based on the photos of their previous stays.

This means that for each Airbnb listing in the dataset, the machine learning model will predict whether it is a suitable recommendation for a user based on their provided photos. It helps users identify accommodations that align with their preferred style and ambiance.

### Features/Predictors for ML Models

Features or predictors are the variables and data points used by the machine learning model to make predictions about the target variable. These features should be relevant and informative in helping the model understand the style preferences of the user and the characteristics of Airbnb listings.

1. **Image Analysis Results:**

   These are features derived from computer vision techniques applied to the photos provided by users. These features might include:
     - Style descriptors (e.g., modern, rustic, minimalist).
     - Color palette information (e.g., warm tones, cool tones).
     - Sentiment analysis (e.g., positive, cozy, vibrant).
     - Object recognition (e.g., presence of a fireplace, pool, beach view).

3. **Property Attributes:**

   Relevant attributes of Airbnb listings, such as:
     - Property type (e.g., apartment, house, villa).
     - Room type (e.g., entire home, private room, shared room).
     - Number of bedrooms and bathrooms.
     - Location or neighborhood.

5. **Pricing Information:** The price of the listing per night or per stay.

6. **Host Information:** Information about the host, such as host responsiveness or Superhost status.

7. **User Preferences:** User-provided preferences, if available (e.g., specific amenities, neighborhood preferences, budget constraints).

8. **Historical Data:** Information about the user's past Airbnb stays, including their previous booking history and any user reviews they have left for other accommodations.
