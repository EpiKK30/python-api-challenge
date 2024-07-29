## WeatherPy & VacationPy: Analyzing Weather Patterns and Planning Vacations

### Overview

This project aims to analyze weather patterns across various global cities and visualize these findings using Python, Pandas, and various APIs. The challenge is divided into two main parts: **WeatherPy** and **VacationPy**.

### Repository Structure

- **WeatherPy**
  - `WeatherPy.ipynb`: Jupyter Notebook for weather data analysis.
  - `api_keys.py`: Contains the API keys (ignored via `.gitignore`).
  - `output_data/cities.csv`: Pre-exported data containing weather information for cities.

- **VacationPy**
  - `VacationPy.ipynb`: Jupyter Notebook for planning vacations using weather data.

### Part 1: WeatherPy

In this part, we explored the relationship between weather variables and latitude. We used the OpenWeatherMap API to gather weather data for over 500 cities.

**Key Tasks:**
1. **Data Collection**: Generated random latitude and longitude pairs and found the nearest city using the Citipy library.
2. **API Integration**: Retrieved weather data for each city using the OpenWeatherMap API.
3. **Data Visualization**: Created scatter plots to showcase the relationships between:
   - Latitude and Temperature
   - Latitude and Humidity
   - Latitude and Cloudiness
   - Latitude and Wind Speed

4. **Linear Regression Analysis**: Computed and visualized linear regressions for each relationship, separately for the Northern and Southern Hemispheres.

**Challenge Faced:**
We unintentionally exceeded our OpenWeatherMap API call limits, which prevented us from acquiring all the necessary data in real-time. To overcome this issue and complete the assignment, we used a previously exported dataset, `cities.csv`, to ensure the analysis could be performed accurately.

### Part 2: VacationPy

In this part, we used the weather data collected in WeatherPy to assist in planning vacations.

**Key Tasks:**
1. **Ideal Weather Criteria**: Filtered the dataset for cities that matched ideal weather conditions.
2. **Hotel Information**: Utilized the Geoapify API to find hotels in these cities.
3. **Mapping**: Created a map visualization with hover functionality to display the city, country, and hotel information.

### Conclusion

This project demonstrated the practical application of data analytics in real-world scenarios such as weather analysis and vacation planning. The limitations faced, such as API call restrictions, highlight the importance of efficient data handling and planning in project execution.

### Future Work

Further exploration could include:
- Implementing additional APIs for more detailed weather predictions.
- Expanding the dataset to include more cities and more diverse geographical regions.
- Automating the data collection process while ensuring compliance with API usage policies.

### Getting Started

1. **Clone the Repository:**
   ```
   git clone <repository_url>
   ```
2. **Install Required Libraries:**
   ```
   pip install -r requirements.txt
   ```
3. **Run the Notebooks:**
   Open `WeatherPy.ipynb` and `VacationPy.ipynb` in Jupyter Notebook to explore the analyses.

### Note

This repository includes a `.gitignore` file to exclude sensitive information such as API keys in `api_keys.py`. Please ensure you have your own API key for OpenWeatherMap and Geoapify to run the notebooks. 

For further questions or contributions, please contact [Kevin Ngala](mailto:kevin.ngala@example.com).

---

This README provides an overview of the WeatherPy and VacationPy project, the challenges faced, and how the issues were resolved. The project demonstrates data analysis and visualization skills, critical for answering practical questions using real-world data.
