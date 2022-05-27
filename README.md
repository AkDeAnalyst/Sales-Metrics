### Nita's SQL Challenge

# A simple project that analyzes sales data 
 
Before you begin, there are a few things you should note.
- Total Average Revenue per Customer (product) = Total Revenue/ Total number of customers (products) 
- Year-Over-Year growth rate = (Total Revenue from current year/ Total Revenue from previous year) – 1
OR (Total Revenue from current year – Total Revenue from previous year) / Total Revenue from previous year
- Take Sales as Revenue (i.e. Sales Revenue); COGS = Profit – Revenue
- To get your year values, make use of the “Ship_date” column (i.e. extract your year from the ship date)
- Asides data cleaning, do not alter the original table (i.e, do not insert or update anything from the original table).
- Some of the tables below are not complete. The purpose of including the tables is to give an idea of what your result should look like.
- The data you will be working with is a super store data gotten from kaggle.com


# Let's begin.

FIRST THINGS FIRST. 
1.	Clean Data. Check for unwanted columns, duplicates, etc. (Free-style, however you want to clean your data)

2.	Find out the Total Average Revenue per Customer and the Total Average Revenue per Product for the year 2017. (return values in 2 decimal places)
  	|Avg_Rev_Customer    |   Avg_Rev_Product |
	|--------------------|-------------------|
	| 1387.45            |    636.35	 |

3.	Give a list of all products that generated revenue below the TAR_Product (Showing the least revenues first)

	    | Product_name 				| Category 	 | Region | Revenue |
	    |-------------------------------------------|----------------|--------|---------|
	    | Acco Suede Grain Vinyl Round Ring Binder  | Office Supplies| Central| 0.556   |

3b. How many of such products fall under the three product categories? Mr. Bid will like to know which category has the most products below the Average Revenue/Product

	   | Region             |    Furniture  | Office_Supplies | Technology  |
	   |--------------------|---------------|-----------------|-------------|
	   |	Central         |  60           |  258            | 51		|
	   |	East            |  85           |  271            | 82		|
	   |	South           |  51           |  159            | 36		|
	   |	West            |  105          |  314            | 82		|


4.	Find out the Y-O-Y growth rate from 2014 – 2017. (Your answer should be rounded to 3 decimal places, and show the “%” sign)
	   | YOY_2015            |     YOY_2016          |       YOY_2017	|
	   |---------------------|-----------------------|----------------------|
	   |	12.492%          |        37.452%        |          14.298	|

5.	Return a table that shows the Total Revenue against the Total Cost of goods sold (COGS) for each region and in each year (2014 – 2017)

	    Year	Rev_East	COGS_East	Rev_West	COGS_West	Rev_South	COGS_South	Rev_Central	COGS_Central
	    -----------------------------------------------------------------------------------------------------------------------------------------
		2014	59565.67496	50621.17028	57056.89765	49639.32618	38249.12705	30295.61321	46774.3888	50681.43272
		2015	75174.10165	63741.23546	72333.43859	63721.54895	36755.28662	35745.82953	42573.09403	38938.8497
		2016	89663.09688	77629.67933	91414.30123	80782.50326	53077.08768	42910.49337	77637.0578	67847.09961
		2017	105900.8682	85908.91383	109936.4272	89413.86001	61748.10101	58637.50291	78787.35225	77074.54872
		2018	395.5859833	348.6923819	1382.706023	1128.229921	1272.623962	971.5423717	550.6919996	425.8050019


        
6.	Return a table that shows the Profit generated per state, then per region in 2018 alone. (Group by region and round off figures to 2 decimal places)
    | State	  | Region  | Profit | Regional_profit |
    |---------|---------|--------|-----------------|
    | Indiana	| Central | 56.51	 | 124.8869976     |
    | Texas 	| Central | 2.72	 | 124.8869976     |
    | New York|	East	  | 12.12	 | 46.89360142     |
    | New York|	East	  | 34.78	 | 46.89360142     |
    | Kentucky|	South	  | 314.04 | 301.0815907     |
    | Tennessee| South	| -12.96 | 301.0815907     |
    | Colorado| West	  | -0.6	 | 254.4761026     |
    | California|	West	| 37.41	 | 254.4761026     |

7.	Return a table that shows the total number of orders received on each day of the week for year 2014, 2015, 2016 and 2017.
	
   | day_of_week | orders14 |   orders15  |  orders16 | orders17   |
   |------------ |----------| ----------- |-----------| -----------|
   | Friday      |    174   |     192     |     242   |      308   |
   | Monday      |    181   |     185     |     242   |      312   |
   | Saturday    |    163   |     168     |     206   |      300   |
   | Sunday      |    146   |     192     |     219   |      293   |
   | Thursday    |    25    |     185     |     249   |      287   |
   | Tuesday     |    177   |     98      |     130   |       53   |
   | Wednesday   |    103   |     18      |     27    |       34   |

