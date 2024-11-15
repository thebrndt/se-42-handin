# README for Spotify Data Analysis

## Project Overview

This project processes and analyzes my user data extracted from Spotify's listening history. The goal is to gain insights into listening patterns and trends. The data is stored in JSON files, which are concatenated and cleaned before analysis.

---

## File Structure

- **`spotify_data.ipynb`**: The primary notebook file that contains all the code for data processing, cleaning, and visualization.
- **`data.zip`**: Contains folders with JSON files representing Spotify listening history and should be extracted before running the notebook.

---

## Data Processing Workflow

1. **Data Loading**:

   - All JSON files in the `my_data/` folder are read and combined into a single Pandas DataFrame after `data.zip` folder is extracted.

2. **Data Cleaning**:

   - Unnecessary columns such as `username`, `ip_addr_decrypted`, and others are dropped.
   - Rows with missing song names (`master_metadata_track_name`) are removed.

3. **Data Analysis**:
   - Analysis focuses on user listening behaviors, including:
     - Most listened-to tracks.
     - Time of day with peak listening activity.
     - Trends in listening over time.
     - Genre preferences (if data contains genre information).

---

## Visualizations

- The notebook utilizes **Matplotlib**, **Seaborn**, and **Plotly** to generate insightful visualizations such as:
  - Bar charts showing top tracks.
  - Line graphs analyzing listening trends over time.
  - Heatmaps for activity distribution across days and hours.

---

## How to Use

1. Extract `data_.zip` folder.
2. Run the notebook `spotify_data.ipynb`.
3. Visualizations and results will be generated for exploratory analysis.

---

## Requirements

- Python libraries:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `plotly`

Install them using:

```bash
pip install pandas numpy matplotlib seaborn plotly

```
