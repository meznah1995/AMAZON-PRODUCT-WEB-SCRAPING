AMAZON PRODUCT WEB SCRAPING

Description
The project code provided is aimed at exploratory web scrapping of product data from the amazon website based on keyword search. The dataset generated on groceries and household items can be used in a variety of analytical projects, example inflation tracking, analysing popular product trends etc., which use the provided parameters in data:
	Description : contains the name and details of the product
	Price : price at the time of scrapping the data
	Rating : rating out of 5
	ReviewCount : number of reviews given for the overall ratings
	Url : link to the product

The code then pre-processes the data based on user requirements like sorting, removing duplicates etc. Python in Jupyter Notebook was used with the Numpy and Panda libraries.

##challenges faced?
* Search terms defer in the amount of pages one can load at a time, for example a search term of 'Queen Mattress' yields 48 page results out of a possible 2000+ while a search term of 'Television' yields 16 page results out of a possible 1000+ results.
* There were no available archive data to include in the daily scrapped data for long term evaluation
## features want to implement in future?
* Continuous data collection for long term evaluation

Usage and Data 
Some points to note for working code are:
	Chrome driver package has to be installed if using Jupyter notebook on Chrome. The foler where the package is saved has to be specified in the address for the driver to function.
	The output csv files generated after scraping will be saved in the same folder as the notebook file and the pre-processing code will access these same files.
	
The provided "data" folder contains CSVs of the raw pre-processed dataset originally sourced from www.amazon.com that has groceries, and household items.
	i. Fresh_meat.csv 
	ii. Fresh_tomatoes.csv 
	iii. Queen_matress.csv 
	iv. Television.csv 
	v. vegan_dairy.csv 
	vi. vegan_grocery.csv 
	vii. vegan_meat.csv  
	viii. Importedreshfruit.csv 
	ix. freshfruit.csv 
	x. freshveg.csv 
	
Processed data were placed in folders:
 'modified'- for sorted data by description and removing advertisement data and duplicates
 'optimal'- for sorted data in descending order considering 'Rating' and 'ReviewCount
 'Sorted_data' - Concatenated and sorted the data for each search term

Supplementary Contents
	1. Project proposal.ipynb
	2. Amazon preprocessing.ipynb
	3. Data folder containing processed data in .csv format.
	4. Presentation
