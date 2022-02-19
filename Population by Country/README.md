README.md

This is my first project!
It is about how the world population has behaved between 1980 and 2010.
The proposal in this work was to apply the basics of data processing. 

First of all I changed the column names creating a list, second I rotated the data frame, turning rows into columns. This made it more intuitive to treat the population size as a function of years.

Thus, it was necessary to create another list, to change the names of the columns again. Now the first column is called "Year" and the remaining ones the name of the countries. 

With the structure organized, now it is time to look at the data. I started looking for holes like "empty" or "NaN" values. But it wasn't enough to cover all the missing values, because the file sometimes used "-" to indicate no register.

After replacing the string "-" with "NaN", I created a pattern to eliminate some countries.
The countries with more or 60% missing data were eliminated. And the missing values of the remaining countries were filled in with the average value of the years. 

After this treatment, I saved it in a csv file, named attachment "pop_country_T" for public use.
