# EXCEL-ASSIGNMENT-2
1) Handling Missing Values:									
	• Check for missing values in the 'Price' column. How would you handle products with missing price information?
In Power Query go to Transform then replace null with median value of prices.
						
	• If there are products with missing categories, propose a strategy to impute or deal with these missing values effectively.
In power query Replace null Values with “Uncategorized” or fill manually.					
									
2) Correcting Inconsistent Data:									
	• Identify any inconsistent text formats present in the "Product Name" column.
Case inconsistencies in product names. There are laptop, Laptop, smartphone, Smartphone, headphones and Headphones.
				
	• Identify any typos present in the "Category" column.
"Electroni" should be "Electronics".
							
	• Use the find and replace function to standardize the text formats in the "Product Name" column and fix any typos or misspellings in the "Category" column.
ctrl + h > Find & Replace > Replace laptop to Laptop, smartphone to Smartphone, headphones to Headphones.
In the "Category" column replace electroni to Electronics.						
									
3) Removing Duplicates:									
	• Identify any duplicate rows within the dataset based on the entirety of each row, and remove them if any.
Select first column then in Power Query > Home > Remove Rows > Remove Duplicates.

4) Splitting and Merging Data:									
	• Split the "Product ID" column into two separate columns for " Manufacturing Date" and "Country Code". Remove unnecessary characters, if any.
	Select Product ID > Transform > Split Column > By Delimiter "-" > Split at rightmost Delimiter. Then rename first part as Manufacturing Date, last part as Country Code.						
	• Merge the "Brand Name" and "Product Name" columns into one column named "Product Brand".
Add Column > Custom Column: =[Brand Name] & " " & [Product Name].
Then rename to Product Brand.								
									
5) Number Formatting:									
	• Format the data type of the "Price" column to currency format.
 In Excel, go to format then format cells to Currency.
								
	• Format the "Manufacturing Date" column to display dates in the "DD-MM-YYYY " format.
 In Excel, go to format then format cells to date in "DD-MM-YYYY " format								
									
6) Conditional Formatting:									
	• Apply data bar or color scales conditional formatting in the "Price" column.
Select column > Home > Conditional Formatting > Data Bars or Color Scales.

• Create a custom rule for conditional formatting in the "Category" column to highlight cells where the category is "Electronics."
Select column > Home > Conditional Formatting > New Rule > Onlu format cell contain > Specific Text > "Electronics"
								
