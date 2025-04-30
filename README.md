# LAPD Crime Data Analysis Tool

This project performs exploratory data analysis (EDA) and visualizations on crime data from Los Angeles, spanning from 2020 to the present. The tool allows users to interactively explore crime trends , patterns by time and location, and the most common types of crimes reported.

## 📂 Dataset

- **Source**: [Crime Data from 2020 to Present](https://data.lacity.org/)
- **Format**: CSV
- **Columns Used**:
  - `Date Rptd`: Date the crime was reported
  - `TIME OCC`: Time of occurrence (HHMM format)
  - `Crm Cd Desc`: Description of the crime
  - `AREA NAME`: Name of the reporting LAPD area

> Make sure the dataset is downloaded and the path is correctly set in the script:
```python
DATA_PATH = "C:\\Users\\hp\\Downloads\\Crime_Data_from_2020_to_Present.csv"
⚙️ Features
✔️ Data Cleaning
Drops rows with missing values in key columns.

Converts Date Rptd to datetime.

Formats TIME OCC into 4-digit strings for consistency.

✔️ Visualizations
Top Crimes: Bar chart of the 10 most common crimes.

Crime Trend Over Time: Monthly line graph of reported crimes.

Crimes by Area: Bar chart of top 10 areas with highest crime counts.

Hourly Crime Distribution: Line graph showing number of crimes by hour.

Area vs Crime Heatmap: Heatmap showing the frequency of top crime types across top LAPD areas.

✔️ Interactive Menu
Run-time console-based interface for exploring various aspects of the data without modifying the code.

▶️ Usage
Install required libraries (if not already installed):

bash
Copy
Edit
pip install pandas numpy matplotlib seaborn
Update the DATA_PATH in the script with your dataset path.

Run the script:

bash
Copy
Edit
python lapd_crime_analysis.py
Choose whether to enter interactive mode or display all visualizations automatically:

vbnet
Copy
Edit
Do you want to run interactive analysis? (y/n):
📊 Example Visuals
Top 10 Most Reported Crimes

Crime Trends Over Time

Note: Replace image URLs with your own if needed.

📁 Folder Structure
bash
Copy
Edit
lapd_crime_analysis/
│
├── lapd_crime_analysis.py       # Main script
├── README.md                    # Project overview
└── Crime_Data_from_2020_to_Present.csv   # Dataset (not included here)
🧠 Future Improvements
Add support for filtering by date range or area.

Export summary statistics to CSV.

Integrate with a simple GUI or web interface (e.g., Streamlit).
