# Conclusion

## 1. Project Overview

The Netflix Analytics project explored a cleaned dataset (earlier raw dataset from Kaggle) containing 8,807 Netflix titles and 14 columns. The main objective was to understand the composition of Netflix's catalogue and identify patterns related to genres, countries, release years, content ratings, movie durations, TV show seasons, actors, directors and content addition dates.

Using Python, Pandas, Matplotlib and exploratory data analysis (EDA), we examined the dataset and presented our findings through graphs and visualizations.

## 2. Data Cleaning: By Prutha Samant

The raw Netflix titles dataset from Kaggle contained 8,807 titles and 12 columns. Before the analysis, it was inspected for data types, missing values, and duplicates. No duplicate rows or duplicate show IDs were found, so no records were removed.

Three issues were corrected. Three titles had their duration stored in the rating column, so those values were moved to the duration column. The date added column was stored as text and was converted to a date format; its 10 missing values were left unchanged because they cannot be recovered from the data. The duration column also mixed minutes and seasons, so it was split into a numeric movie duration column (6,131 movies) and a seasons column (2,676 TV shows), which is why the cleaned dataset has 14 columns.

Missing director (2,634), cast (825) and country (831) values were filled with **Unknown** so that no titles were lost. The cleaned dataset was validated, saved as data/cleaned/netflix_cleaned.csv and shared with the team through a separate branch and pull request.

This gave the team a consistent dataset containing all 8,807 titles to work from.

## 3. Key Findings from the Analysis
### 3.1 Country-wise Analysis: By Sania Redkar
- **Genre Analysis**

The genre analysis identified **International Movies** as the most frequent genre. This highlights the significant representation of international movie content in the dataset.

- **Country-wise Analysis**

The United States ranked first in the country-wise content analysis. It also had the highest number of unique actors associated with its content in our country-actor analysis.

These findings show that the United States has a significant representation in the Netflix dataset.

### 3.2 Content Analysis: By Pranaya Gaonkar
- **Movie Duration Analysis**

The average movie duration was approximately **99.56 minutes**. The shortest movie recorded was 3 minutes while the longest was 312 minutes.

This analysis helped us understand the range of movie durations represented in the dataset.

- **TV Show Seasons Analysis**

The average number of seasons for TV shows was **1.76**, while the median was one season. The most common category was one-season shows with 1,793 titles.

This indicates that single-season shows were the most frequently represented category in our TV show seasons analysis.

- **Content Added by Month**

The monthly analysis showed that **July had the highest number of movies added**, with 565 titles, while **December had the highest number of TV shows added**, with 266 titles.

This helped us compare the monthly distribution of movies and TV shows added to Netflix.

- **Content Age Classification**

The content age analysis classified 63.08% of the eligible titles as recent, meaning they had a release-to-addition gap of 0–2 years. Another 12.74% were classified as moderately older, with a gap of 3–5 years, while 24.18% had a gap of more than five years.

This provided another way to understand the distribution of titles according to the time between release and addition.

### 3.3 Overall Visualization: By Sanika Verlekar
- **Release Year Analysis**

The release year analysis showed that the number of Netflix titles increased significantly over time especially after 2000. The highest number of titles was observed around 2018, with approximately 1,150 titles.

This helped us understand the growth of Netflix's content library and identify trends in title releases.

- **Content Rating Analysis**

The content rating analysis showed that TV-MA was the most common rating, with approximately 3,200 titles, followed by TV-14 with around 2,150 titles. Other ratings, such as TV-PG and R, were also present in significant numbers.

This helped us understand the distribution of Netflix titles according to their intended audience and content ratings.

- **Actor and Director Analysis**

The actor analysis identified Anupam Kher as the most frequently listed actor in the results, appearing in 43 titles. The director analysis identified Rajiv Chilaka as the director associated with the highest number of titles, with 22 titles.

These results helped us explore the contributions of actors and directors represented in the dataset.

- **Other Visualizations**

We also created visualizations showing the distribution of movies and TV shows, release years, content ratings and ratings by content type. These graphs provided additional ways to explore the structure and characteristics of Netflix's catalogue.

## 4. Overall Conclusion

The project provided useful insights into the composition of Netflix's catalogue. Our analysis identified International Movies as the most frequent genre, the United States as the leading country in the country-wise analysis and one season as the most common TV show season count. We also examined movie durations, monthly content additions, content age classification and the representation of actors and directors.

The project helped us apply data cleaning, exploratory data analysis and data visualization techniques to a real world dataset. It also gave us practical experience in organizing a collaborative project using Git, GitHub and Markdown.

## 5. Limitations
The cleaning process kept every title, so 831 titles have an **Unknown** country and the rating and date added fields remain missing for 7 and 10 titles respectively. The cast, country and genre columns also still contain several comma-separated values per cell and need to be split before analysis.

The dataset contains missing or unknown information for certain attributes, including country, cast and director. Therefore some analysis were limited to available records and the results depend on how missing values were handled.

Additionally the dataset describes Netflix titles and their attributes, it does not directly measure viewership, popularity or audience satisfaction. The findings should therefore be interpreted as observations about the dataset rather than conclusions about audience preferences.

## 6. Future Scope

The project could be extended by exploring more detailed genre and release-year trends, examining relationships between content ratings and content types, and improving the visual presentation of the findings.

Future analysis could also use additional data about viewership and audience engagement to investigate how the characteristics of Netflix titles relate to their performance.

**(Documentation and GitHub handling by Pranjali Marshelkar)**

