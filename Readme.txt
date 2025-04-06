# Air Quality Analysis & Visualization Tool (Python Executable)

This Python-based tool is designed for environmental professionals and researchers to perform quick analysis and visualization of air quality CAAQMS datasets — without needing to write code, even rename downloaded file, or sort data, or even work on excel.



## 🚀 Usage

1. **Run the executable (.exe application file)**
   - The program uses a graphical interface, so no command-line input is required.

2. **Prompt: "Select your data file."**
   - A file dialog will open to select your Excel or CSV file containing the data.
   - Required structure: Excel file downloaded from CAAQMS portal- both types current year and historical data


3. Output: `<Station_name>_<City_name>_SummaryTable.xlsx`
   - saved in the path where provided CAAQMS_data file is stored.
   

4. **Prompt: "Select Pollutants for Hourly Average Plot"**
    - Above prompt will give list of available pollutants- Enter pollutant names separated by commas if selecting more than one.
    - Output-<Station_name>_<City_name>_<Pollutant_name>_Hourly_Variations_Plot.jpg


5. **Prompt: "Dataset selection- Enter 'hourly' for plots on hour wise distribution data, or 'whole' for plots on entire dataset"**
    - It will convert data into hourly average if entered 'hourly' and then plots box or violin, otherwise if eneterd 'whole' it will plot on the actual data provided.
  
6. **Prompt: “Enter 'box' for Box Plot or 'violin' for Violin Plot"
    - Output-<Station_name>_<City_name>_<DatasetSelection-Whole/Hourly>_<PlotType-Violin?Box>-Plot.jpg`


5. **Prompt: “Do you want a line plot? (yes/no)”**
   - Enter `yes` to generate time series line plots.
   - Next prompt: Choose `all` to plot all pollutants or list specific ones separated by commas.
   - For each pollutant:
     - Plot saved as: `<station_name>_<city_name>_<pollutant>_Line_Plot.jpg`
   - If `all` is selected:
     - Combined plot saved as: `<station_name>_<city_name>_All_Pollutants_Line_Plot.jpg`

6. **Prompt: “Do you want to create an infographic? (yes/no)”**
   - Enter `yes` to build a custom infographic.

7. **Infographic Customization Prompts:**
   - Enter title for infographic.- Type or copy main title to be put in the infographic
   - Enter subtitle.- Type or copy subtitle to be put below main title in the infographic
   - Enter first paragraph (required).- Type or copy description you want to write in left half side of infographic
   - Enter second paragraph (optional).- Type or copy description you want to write below first paragraph.
   - Select background image (optional).- Select file which will be used in the background of infographic.
   - Select up to 3 plot images (optional, recommended from the earlier outputs).- Select file one by one to be put in right half side of infographic one above another.

8. **Infographic Output:**
   - Final styled image saved as: `final_infographic.png`
   - Saved in the same directory as the script or `.exe`.