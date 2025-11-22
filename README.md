# **🎬 Amazon Prime Video EDA Project**

## **📌 Overview**
This project focuses on performing an in-depth Exploratory Data Analysis (EDA) on the Amazon Prime Video Titles and Credits datasets. The goal is to understand how Amazon Prime's content is structured, how it has grown over time, and what factors influence popularity and ratings. Through data cleaning, feature engineering, and visual exploration, this project uncovers key trends related to genres, release years, cast information, user ratings, and viewer engagement metrics.

## **🗂 Dataset**
#### ***The project uses two main datasets:***
- titles.csv → Contains information about each movie or TV show such as title, description, genres, runtime, ratings, release year, and popularity metrics.

- credits.csv → Contains cast and crew information including person IDs, names, character roles, and credit type (ACTOR / DIRECTOR).

After preprocessing and merging on the id column, a final processed file named merged_df.csv is generated and used for analysis.

## **🧹 Data Preparation & Cleaning**
#### ***A complete data cleaning pipeline was performed, which included:***
- Handling missing values using appropriate replacements (median, 0, “Not Rated”, etc.)
- Removing inconsistent formats and fixing column types
- Merging both datasets into one consolidated table
- Aggregating cast and character details for each title
- Creating useful new features such as:
    -> decade – The decade a title was released
    -> genres_list – A cleaned list of genres
    -> primary_genre – The main genre of each title

These steps ensured the final dataset was clean, complete, and ready for visual analysis.

## **📊 Visualizations (25+)**
#### ***The EDA was structured using the UBM framework:***
🔹 **Univariate Analysis**

    - Genre distribution
    - IMDb score distribution
    - Runtime histogram
    - Popularity and votes distribution
    - Age certification breakdown
    - Production country counts

🔹 **Bivariate Analysis**

    - Runtime vs IMDb score
    - Votes vs rating
    - Popularity vs votes
    - Score vs primary genre
    - Type (Movie/TV) vs decade

🔹 **Multivariate Analysis**

    - Correlation heatmaps
    - Pairplots
    - Bubble charts
    - Genre vs seasons heatmap
    - Score quartile comparison

These charts helped understand relationships between different features and identify meaningful patterns.  

## **💡Key Insights**

- A majority of titles were released after 2010, showing rapid recent growth in Prime Video’s catalog.
- Drama and Comedy are the most common genres, dominating the platform’s content library.
- IMDb scores mostly lie around 6, indicating moderate overall content quality.
- Popularity is highly skewed, meaning only a small group of titles receive massive engagement.
- Movies make up most of the dataset, while TV shows contribute strongly to user retention.
- Some metadata fields such as age certification and cast information have noticeable missing values.  

## **📈 Business Recommendations**

#### ***Based on the insights, the following suggestions can help improve Prime Video’s content strategy:***

- Promote and highlight top-performing titles to boost engagement and viewership.
- Improve metadata completeness, especially ratings and cast details, to enhance search and recommendations.
- Invest more in TV shows, as they have high retention potential.
- Explore underrepresented genres and regions to increase content diversity.
- Utilize popularity and votes as strong indicators for marketing and content acquisition decisions.  

## **🛠 Tech Stack & Libraries**

--->> Python
--->> Pandas – Data cleaning and manipulation
--->> NumPy – Numerical operations
--->> Matplotlib – Visualizations
--->> Seaborn – Statistical plots and styling
--->> Jupyter Notebook – Analysis environment  

## **🏁 Conclusion**
This EDA project successfully combines the Titles and Credits datasets to uncover important patterns in Amazon Prime Video's content. The analysis provides valuable insights into genre trends, content availability, user engagement, and popularity. These findings can help guide decisions related to content acquisition, personalized recommendations, marketing strategy, and user experience improvements. Overall, the project demonstrates a complete end-to-end EDA workflow, from data cleaning to visual insights, and lays the foundation for more advanced analytics or predictive modeling in the future.
