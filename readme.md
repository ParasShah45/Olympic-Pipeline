# EDA Project

# Olympic Games Data Analysis

## Project Overview

This project performs Exploratory Data Analysis (EDA) on the Olympic Games dataset to uncover trends in athlete participation, medal distribution, sports events, and demographic characteristics.

The analysis was conducted using Python and various data analysis libraries to gain insights into historical Olympic performance and participation patterns.


## Objectives

- Analyze athlete participation over the years.
- Explore gender distribution in Olympic events.
- Study age, height, and weight characteristics of athletes.
- Examine medal distribution across competitions.
- Identify sports with the highest number of events.
- Discover country-level participation trends.


## Dataset

The dataset contains historical Olympic athlete records including:

- Athlete Name
- Gender
- Age
- Height
- Weight
- Team
- Country (NOC)
- Sport
- Event
- Medal
- Year
- Season


## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook


## Data Cleaning Steps

- Checked missing values
- Removed duplicate records
- Performed data type validation
- Generated descriptive statistics
- Conducted exploratory analysis


## Key Insights

### Olympic Participation Growth
- Athlete participation has increased significantly over the years, reflecting the global expansion of the Olympic Games.

### Gender Representation
- Male athletes historically dominated participation, but female participation has steadily increased.

### Medal Distribution
- Gold, Silver, and Bronze medals show expected distribution patterns across Olympic events.

### Sports Diversity
- Certain sports contain significantly more events than others, contributing heavily to overall participation.

### Athlete Demographics
- Most athletes fall within a competitive age range, with noticeable differences across Olympic seasons.


## key Findings

### Athlete Participation Trend
- year_participant_count = df.groupby("Year")["ID"].nunique()

### Sports with Most Events
- sport_event_count = df.groupby("Sport")["Event"].nunique()

### Country with Most Medal Winners
- most_medal_country = df["NOC"].value_counts().idxmax()

### Average Athlete Age by Year
- year_avg_age = df.groupby("Year")["Age"].mean()

### Gold Medal Count by Country
- country_gold_medals = (
    df[df["Medal"]=="Gold"]
      .groupby("NOC")["Medal"]
      .count()
)


## Visualizations

- Olympic Participation Trend
- Gender Distribution of Athletes
- Medal Distribution Analysis
- Top Sports by Number of Events
- Athlete Age Distribution
- Age Distribution by Season
- Top Countries by Average Athlete Age


## Future Improvements

- Interactive Dashboard using Power BI
- Olympic Medal Prediction Model
- Country Performance Analysis
- Athlete Performance Trends


## Project Structure

Olympic-Data-Analysis/
│
├── dataset/
│ └── dataset_olympics.csv
│
├── notebooks/
│ └── Olympic.ipynb
│
├── images/
│ ├── participation_trend.png
│ ├── medal_distribution.png
│ ├── gender_distribution.png
│ └── top_sports.png
│
├── README.md
└── requirements.txt

