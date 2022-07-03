## __ESO Crafting Material Prices__

For my Code Kentucky Data Analysis 1 project I'll be looking at the price history of comparable crafting materials in the MMORPG *The Elder Scrolls Online*. The materials chosen are all used in similar ways with similar sources, but have had dramatically different price fluctuations over the years. All items are sold by players via shop locations purchased by player-created guilds, and a third party add-on (Tamriel Trade Centre) manages a searchable database of listings. TTC uses their database to create price suggestions for players, and their daily suggestions were used for getting the price for each date, along with the number of listings and total quantity listed for most dates tracked.

### __Data__

Prices were recorded by me from the Tamriel Trade Centre add-on and website (https://us.tamrieltradecentre.com/pc/Trade). Each date includes the suggested price ranges for the PCNA server only. 

### __Project Plan__

#### Feature 1: Read data in.

Data will be read from a csv via pandas read_csv function in a Jupyter Notebook.

#### Feature 2: Manipulate and clean your data.

Date formatting will be adjusted for consistency and usability, and unneccessary sections of data will be removed.

#### Feature 3: Analyze your data.

I intend to find the mean, median, and mode of a price within the tracked time period. I also intend to find the highest and lowest prices per item, and calculate how much the price changed before and during known in-game events and patches that affected availability and demand.

#### Feature 4: Visualize your data.

Matplotlib will be used to create a line graph of prices over a bar graph of available quantity of an item over time. Similar graphs of different items will be created for comparison.

#### Feature 5: Interpret your data and graphical output.

Obvious interpretations will be discussed, along with possible explanations (temporary changes to drop rate or demand from in-game events, for example), in markdown cells throughout the notebook.