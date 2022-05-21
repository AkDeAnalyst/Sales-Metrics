### Sales-Metrics

# A simple project that analyzes sales data 
 
Before you begin, there are a few things you should note.
- Total Average Revenue per Customer (product) = Total Revenue/ Total number of customers (products) 
- Year-Over-Year growth rate = (Total Revenue from current year/ Total Revenue from previous year) – 1
OR (Total Revenue from current year – Total Revenue from previous year) / Total Revenue from previous year
- Revenue = sales * quantity; COGS = Profit – Revenue
- To get your year values, make use of the “Ship_date” column (i.e. extract your year from the ship date)
- Whatever you do, the original table should not be altered (i.e, do not insert or update anything from the original table.
- Some of the tables below are not complete. The purpose of including the tables is to give an idea of what your result should look like.
- The data you will be working with is a super store data gotten from kaggle.com


# Let's begin.

FIRST THINGS FIRST. 
1.	Clean Data. Check for unwanted columns, duplicates, etc. (Free-style, however you want to clean your data)

2.	Find out the Total Average Revenue per Customer and the Total Average Revenue per Product for the year 2017. (return values in 2 decimal places)
  	| Avg_Rev_Customer | Avg_Rev_Product |
    |------------------|-----------------|
    | 6986.15          | 3204.18         |

3.	Give a list of all products that generated revenue below the TAR_Product (Showing the least revenues first)
    | Product_name | Category | Region | Revenue |
    |--------------|----------|--------|---------|
    | Acco Suede Grain Vinyl Round Ring Binder | Office Supplies | Central | 0.556 |

3b. How many of such products fall under the three product categories? Mr. Bid will like to know which category has the most products below the Average Revenue/Product

    | Region       | Furniture  | Office_Supply | Technology |
    |--------------|------------|---------------|------------|
    | Central      | 59         | 261           | 51         |
    | East         | 84         | 271           | 82         |
    | South        | 57         | 159           | 42         |
    | West         | 102        | 315           | 82         |

4.	Find out the Y-O-Y growth rate from 2014 – 2017. (Your answer should be rounded to 3 decimal places, and show the “%” sign)
    | YOY_2015      | YOY_2016    | YOY_2017 |
    |---------------|-------------|----------| 
    | 14.558%       | 32.446%     | 6.301%   |  

5.	Return a table that shows the Total Revenue against the Total Cost of goods sold (COGS) for each region and in each year (2014 – 2017)
    | Year | Revenue_East | COGS_East | Revenue_West | COGS_West | Revenue_South | COGS_South | Revenue_Central | COGS_Central |
    |------|--------------|-----------|--------------|-----------|---------------|------------|-----------------|--------------|
    | 2014 | 304593.1	    | 295648.6	| 300935.8	   | 293518.2	 | 208933.9	     | 200980.4	  | 232004.6	      | 235911.6     |          
    | 2015 | 396886.6	    | 385453.8	| 387629.3	   | 379017.4  | 219927.7	     | 218918.3	  | 194376.3	      | 190742       |
    | 2016 | 424248.5	    | 412215.1	| 423828.9	   | 413197.1	 | 264221	       | 254054.4	  | 475498.9	      | 465708.9     |
    | 2017 | 507553.2	    | 487561.2	| 555322.1	   | 534799.6	 | 288495.3	     | 281775.4	  | 336479.6	      | 334766.8     |
        
6.	Return a table that shows the Profit generated by per state, then per region. (Group by region and round off figures to 2 decimal places)
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

