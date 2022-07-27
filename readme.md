# __*The Elder Scrolls Online* Furnishing Material Prices__

For my Code Kentucky Data Analysis 1 project I'll be looking at the price history of comparable crafting materials in the *The Elder Scrolls Online*. The materials chosen are all used in similar ways with similar sources, but have had dramatically different price fluctuations over the years. 

## __Data__

All data before March 2022 was taken from the Tamriel Trade Center add-on for ESO. Once Tamriel Trade Center's website (https://us.tamrieltradecentre.com/pc/Trade/PriceCheck) began including the price history for each item, most entries were recorded using the website rather than the in-game item tooltip. Prices may be rounded differently depending on the source. TTC's suggested price ranges (included in the csv) were simplified by finding the mean of the upper and lower values in Google Sheets.

Due to an issue with the add-on recording duplicates after scanning trader listings, number of listings and total quantity listed for 1-16-21 and 1-19-21 were manually adjusted to be in line with other entries and quantity values for those dates are likely still inaccurate.

## __Setup__

Download repository from GitHub. 
Main file is a Jupyter Notebook. Install Anaconda (http://www.anaconda.com), then open 'ESOMatPrices.ipynb'

#### __Packages needed:__

- pandas
- numpy
- matplotlib

## __Project Plan__

#### Feature 1: Read data in.

Data is read using pandas read_csv function.

#### Feature 2: Manipulate and clean your data.

- Used dropna to remove missing values
- Used filter to select specific columns from the csv
- Used pandas concat to merge results into a dataframe
- Renamed columns for readability
- Rounded results for readability

#### Feature 3: Analyze your data.

- Pandas min for the minimum value
- Pandas idxmin for the index (date) of the minimum value
- Pandas max for the maximum value
- Pandas idxmax for the index (date) of the maximum value
- Pandas diff for the difference between a row and the previous row
- Pandas desc for descriptive statistics

#### Feature 4: Visualize your data.

- Table of min/max + index results (2020 vs 2022)
- Line graphs showing price in 2019, 2020, and 2022
- Line graph of quantity in 2020 and 2022
- Multiple graphs with shared x-axis and separate y-axis scales for comparing changes in price and quantity per item

#### Feature 5: Interpret your data and graphical output.

Obvious interpretations are discussed, along with the most likely explanations (in-game events and patches, etc), in markdown cells throughout the notebook. Any unexplained price changes are discussed in the context of the item's use and the game's economy.

#### __Changes from Project Plan__

Used pandas descriptive statistics function instead of mean, median, and mode.