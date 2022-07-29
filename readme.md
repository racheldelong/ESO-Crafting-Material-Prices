# __*The Elder Scrolls Online* Crafting Material Prices__

For my Code Kentucky Data Analysis 1 project I'll be analyzing the price of furniture crafting materials in *The Elder Scrolls Online*. The materials are all used in similar ways with similar sources, but have had dramatically different price fluctuations since 2019.


## __Data__

Entries before March 2022 were obtained from the [Tamriel Trade Center](https://us.tamrieltradecentre.com/) add-on for ESO. Once Tamriel Trade Center's website added the price history for each item, most entries were recorded using the website rather than the in-game item tooltip supplied by the add-on. Prices may be rounded differently depending on the source. TTC's suggested price ranges on each date (included in the csv) were simplified by finding the mean of the upper and lower values in Google Sheets.

Due to an issue with TTC's website listing duplicates, the number of listings and total quantity listed for January 16th & 19th, 2021 were manually adjusted to be in line with other entries and quantity values for those dates are likely still inaccurate.


## __Setup__

Clone repository from GitHub. 

Install [Anaconda](https://docs.anaconda.com/anaconda/install/index.html), and run the 'ESOMatPrices.ipynb' Jupyter Notebook.

#### __Packages used:__

- pandas
- numpy
- matplotlib


## __Project Plan__

#### __Feature 1: Read data in.__

Data is read using pandas read_csv function.

#### __Feature 2: Manipulate and clean your data.__

- Used dropna to remove missing values
- Used filter to select specific columns from the csv
- Used pandas concat to merge results into a dataframe
- Renamed columns for readability

#### __Feature 3: Analyze your data.__

- Pandas min for the minimum value
- Pandas idxmin for the index (date) of the minimum value
- Pandas max for the maximum value
- Pandas idxmax for the index (date) of the maximum value
- Pandas diff for the difference between a row and the previous row

#### __Feature 4: Visualize your data.__

- Table of minimum and maximum results, with date (2020 vs 2022)
- Line graph showing price in 2019, 2020-21, and 2022
- Line graph of quantity in 2020-21 and 2022
- Multiple graphs with shared x-axis and separate y-axis scales for comparing changes in price and quantity per item

#### __Feature 5: Interpret your data and graphical output.__

Obvious interpretations are discussed, along with the most likely explanations (in-game events and patches, etc), in markdown cells throughout the notebook. Any unexplained price changes are discussed in the context of the game's economy.

#### __Changes from Project Plan__

Used minimum, minimum index, maximum, maximum index, and difference instead of mean, median and mode, to focus on when changes occurred.


![](https://i.imgur.com/Un3PPMr.jpg)
