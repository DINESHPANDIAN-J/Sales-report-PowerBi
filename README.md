# Sales-report-PowerBi
Here  have Created a Report On Sales Data.
 Data Available:
1.	Sales (folder contains sales data of different years)
2.	Categories (Excel having Different Categories In a dataset)
3.	Geography ( file has place  where the sales has been done)
4.	Product (Csv file having descryption about Prouct)
5.	SalesRep (Excel files having information about Sales rep)
6.	SubCategories (Excel file having Sub Categories list)
Data Modeling:
•	In Sales folder I have imported the folder so that in future if newyear data comes it will be synchronized.
•	In sales file Country and city where given under single column,for that I have given number to the unique combination of Country and city as “Geokey”.
•	In sales rep file , found some Duplicated IDs cleaned them to have unique Values.
•	Have Created a “DateMaster” table to have Month_no,Month_name,week_no,week_name and quarter_no to make analysis Better.
DAX Calculation:
	Calculated Total Revenue in Sales table, using the Product’s Retail Price, and multiplying it by the Units.(by using Related function because “Unit” in sales table &”RetailPrice” in product table.)
	Calculated Total Cost in Sales table, using the Product’s Standard Cost, and multiplying it by the Units.
	Calculated Gross Profit in Sales: Total Revenue – Total Cost
	Calculated a Gross profit MoM growth Change% measure that could be benefit in decision making
	Calculated a measure for AVG sales per day – this is the average sum of Total Revenue per day based on the Dates of actual Sales.	
Calculate the following time measures:
	Month on Month analysis & Quarter on Quarter analysis has done on Total Revenue
Charts:
•	I have used Water fall chart to get Total Revenue by Product Name & Year.Here I have Locked the “Water fall Chart” with Resect to the “Year Card” . Because if  select only one year means the total revenue by Product name and year break down for the Paricular year only which I don’t want.
