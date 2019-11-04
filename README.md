# SHARK-ATTACKS-ANALYSIS
Analysis of the shark attacks thata ended in deaths from 1985

In this analysis I am cleaning the dataframe from repeated columns, droping columns not relevant to the analysis and grouping the attacks by  new column called Continent.

I will be working with the pandas library

# Importing the data

After importing the pandas lybrary, I import the csv

# Checking columns

I am droping 'Case Number.1' and 'Case Number.2' after checking they are both exactly the same as 'Case Number'.

I am also droping a series of columns that are not relevant to calculate the number of deaths by 'Country', such as 'Date', 'Location', 'Name' and others.

# Filtering data

I am now eliminating all the rows of attacks that weren't Fatal. For that, I take the 'Fatal(Y/N)' column and set all its values to 'Y' or 'N'.

Then I drop those with a value different to Y in the column

I also drop all the rows with 'Year' smaller than 1985

# Adding new column Continent

I first print the set of 'Country'. Then, I create list of continents and split the set between them.

I import numpy to create a new empty column 'Continent'.

Then, I fill continent depending on wether the elements of each continent list contains the 'Country' in each row.

After that, I check the number of null values and find a row without 'Continent'. I solve it.

# Creating Male and Female

I create new columns 'Male' and 'Female' and assign to them a value depending on the 'Sex ' column.

# Group by Continent

Finally, I create a new dataframe df2 and I group it by continent, and aggregate the count of country and 'Male' and 'Female'.

# Bonus

I create a graphic showing the deadly attacks by continent and sex
