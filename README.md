# EDA
# Zomato Restaurant Data Analysis

This project performs exploratory data analysis (EDA) on a dataset containing information about restaurants listed on Zomato. The analysis includes understanding the restaurant distribution across various countries, identifying popular cities for Zomato orders, analyzing ratings and online delivery availability, and drawing insights from the restaurant data.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)
- [Exploratory Data Analysis](#exploratory-data-analysis)
  - [Country-wise Distribution](#country-wise-distribution)
  - [Rating Analysis](#rating-analysis)
  - [Online Delivery Availability](#online-delivery-availability)
  - [City-wise Distribution](#city-wise-distribution)
- [Observations](#observations)
- [How to Run the Project](#how-to-run-the-project)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

This project utilizes a Zomato dataset, which contains various features related to restaurants, including their locations, cuisines, ratings, and availability of services such as online delivery and table booking. The primary goal of this project is to extract meaningful insights from the data to better understand Zomato's global presence, the restaurant ratings distribution, and the availability of services.

## Dataset

The dataset used for this analysis consists of two files:
1. **zomato.csv**: Contains information about restaurants, including location, cuisine, ratings, and service availability.
2. **Country-Code.xlsx**: Maps the country codes to their respective country names.

Key columns in the Zomato dataset include:
- `Restaurant ID`: Unique identifier for each restaurant.
- `Restaurant Name`: Name of the restaurant.
- `Country Code`: The country where the restaurant is located.
- `City`: The city of the restaurant.
- `Cuisines`: The types of cuisine the restaurant offers.
- `Average Cost for two`: The average cost for two people to dine at the restaurant.
- `Aggregate rating`: The overall rating of the restaurant.
- `Votes`: Number of votes or reviews for the restaurant.
- `Has Table booking`: Indicates if the restaurant allows table booking.
- `Has Online delivery`: Indicates if the restaurant offers online delivery.
- `Rating color`: Color coding for the restaurant’s rating.

## Technologies Used

- **Python**: Programming language used for data analysis.
- **Pandas**: For data manipulation and analysis.
- **Matplotlib**: For data visualization.
- **Seaborn**: For enhanced data visualizations.
- **NumPy**: For numerical computations.

## Exploratory Data Analysis

The following analyses were conducted on the dataset:

### Country-wise Distribution

The analysis starts by mapping the `Country Code` to their respective country names using the `Country-Code.xlsx` file. The following key insights were found:
- **India** contributes to the majority of the restaurant listings with approximately 94.39% of the entries.
- **United States** and **United Kingdom** follow with 4.73% and 0.87%, respectively.
- A pie chart is used to visualize the country-wise distribution of restaurant listings.

### Rating Analysis

The dataset provides `Aggregate rating`, `Rating color`, and `Rating text` for each restaurant, allowing an analysis of the rating distribution:
- A significant portion of the restaurants have an aggregate rating of 4.0 and above, categorized as "Very Good" or "Excellent."
- There is a sizable portion of restaurants that have not been rated yet (`Aggregate rating` of 0.0).
- The ratings were visualized using bar plots, showing the distribution of rating counts across different rating categories.

### Online Delivery Availability

A key feature of interest is whether a restaurant offers online delivery. The analysis shows:
- **India** has the highest number of restaurants offering online delivery.
- The **UAE** is the only other country with a significant number of restaurants offering online delivery.

### City-wise Distribution

The dataset also includes the cities where the restaurants are located. The analysis revealed:
- **New Delhi**, **Gurgaon**, and **Noida** are the top three cities with the most restaurant listings.
- The majority of the cities with Zomato listings are from the Delhi region.

## Observations

1. **India** has the overwhelming majority of restaurant listings in the dataset. Zomato’s presence in the **United States** and **United Kingdom** is relatively small in comparison.
2. The majority of restaurants in the dataset offer **high ratings** (above 4.0), especially those in the **Excellent** and **Very Good** categories.
3. Online delivery services are mostly offered in **India** and to a smaller extent in the **UAE**.
4. **Delhi NCR** (New Delhi, Gurgaon, Noida, Faridabad, Ghaziabad) is the most prominent region for Zomato orders, indicating the platform’s dominance in this geographical area.

## How to Run the Project

### Prerequisites
- Python 3.x installed on your local machine.
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`.

### Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/akhileshkrsingh1/EDA
    cd zomato-analysis
    ```

2. Install the required Python libraries:
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```

3. Download the dataset:
   - Place `zomato.csv` and `Country-Code.xlsx` in the project directory.

### Running the Code
To run the analysis, execute the Python script:
```bash
python zomato_analysis.py
