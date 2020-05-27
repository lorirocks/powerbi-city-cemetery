Purpose: First independent Power BI Dashboard
Data: Nashville City Cemetery - Looking only at 1849-1850 cholera epidemic


Nashville cholera deaths happened **Jan. 1849** through **July 1850**

**DATA CLEANING**
To get range of dates: Used DATE function to combine three separate columns, Month No., Burial Day, Burail Year into mm/dd/yyyy  
 =DATE([@[Burial Year]],[@[Month No.]],[@[Burial Day]])
Then copied/pasted data as Value
Then added Cholera Epidemic boolean column for Jan.1849 through July.1850 to look only at deaths in that date range (including those who died of other causes)   
NOT LOOKING at deaths on any other dates in this query.  

To get Cholera and diahrrea in all of their spellings, added two new T/F columns (one for each), and used IF statement to put True/False if name appeared in the previously cleaned COD_Corrected column.



**From Wikipedia**

Nashville, Tennessee cholera epidemic (1849–1850)
From Wikipedia, the free encyclopedia

A cholera epidemic began in Nashville, Tennessee, in January 1849 and caused many deaths in the city in 1849 and 1850.

The Nashville cholera epidemic was part of the third cholera pandemic that occurred between 1846 and 1860. It began in South Asia and was spread globally by travelers. In the United States, the disease outbreak was first recorded in December 1848 at two ports: New York City on December 2 and New Orleans on December 11. It spread into the interior of the country along waterways, **appearing in Nashville on January 20, 1849**.

**The number of cases increased by June 1849**. The death that month, in Nashville, of former president James K. Polk may have been due to cholera, possibly acquired during travels in other parts of the South. Cholera is reported to have been prevalent in the city around the time of his funeral, in June 1849. According to an account published in 1866, there were **311 cholera deaths in Nashville in 1849**, a very large death toll for a city with a population of only about 10,000.  


**The number of cases increased dramatically again in June and July 1850. Estimates of cholera deaths in 1850 range from 316 to about 500. There were 64 deaths from cholera in just the first 4 days of July 1850.** The epidemic led the University of Nashville to suspend operations and led its president, Philip Lindsley, to resign. In a letter written on July 16, 1850, Mary Hamilton House reported to her husband that the epidemic was waning, as the death rate had dropped to only "three to six or eight deaths" per day. The following month, mineralogist Gerard Troost died in Nashville from cholera.

https://en.wikipedia.org/wiki/Nashville,_Tennessee_cholera_epidemic_(1849%E2%80%931850)


*NOTE FROM LORI: 
1849 = 311 deaths
1850 = 500 deaths
TOTAL  811 deaths

That's 3.11%    
CURRENT POPULATION as of mid-2019 is 670,000. If 3.11% died of a disease today that would be 20,837 people in 18 months.  
PERSPECTIVE: Current Davidson County Deaths from COVID-19 AS OF 4/28/2020 is 25.*  