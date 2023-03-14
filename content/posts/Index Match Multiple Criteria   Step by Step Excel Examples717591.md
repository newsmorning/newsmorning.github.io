---
title: "Revolutionize Your Excel Skills with These Index Match Multiple Criteria Techniques - Complete with Step-by-Step Examples!"
ShowToc: true 
date: "2022-12-06"
author: "Kristie Mcfadden"
---
*****
# Revolutionize Your Excel Skills with These Index Match Multiple Criteria Techniques - Complete with Step-by-Step Examples!

Are you tired of struggling with endless VLOOKUP formulas that don't quite fit the bill? Do you need to find a way to search through massive data sets and retrieve specific information in a more efficient manner? Then look no further than the Index Match Multiple Criteria technique in Excel!

With this powerful Excel tool, you can easily search through your data sets and retrieve specific information based on multiple criteria. By combining the INDEX and MATCH functions, you can create a more flexible and dynamic search formula that can handle complex data sets with ease.

In this article, we'll walk you through the process of using Index Match Multiple Criteria in Excel, and highlight some of the key benefits of this approach. We'll also provide you with step-by-step examples to help you get started using this powerful Excel tool.

# Step 1: Understanding the Basics

Before diving into the specifics of Index Match Multiple Criteria, it's important to understand the fundamentals of the INDEX and MATCH functions.

* INDEX: The INDEX function returns a value or reference to a cell within a specified range based on a specified row and column number.
* MATCH: The MATCH function returns the position of a specified value in a specified range of cells.

By combining these two functions, you can create a formula that searches for specific data based on multiple criteria.

# Step 2: Creating Your Formula

To begin using the Index Match Multiple Criteria technique, you'll need to create a formula that combines the INDEX and MATCH functions. Here's an example:

INDEX(range,MATCH(1,(criteria1=range1)*(criteria2=range2),0))

In this formula, "range" refers to the range of cells you want to search through, while "criteria1" and "criteria2" refer to the specific criteria you're looking for. To explain this in layman's terms, let's say you're looking for a specific value in a table with multiple columns and rows. Here's how you'd use the formula:

* Identify the range of cells you want the formula to search through.
* Identify the two criteria that must be met in order to retrieve your desired value.
* Use the INDEX function to return a value or reference within the specified range.
* Use the MATCH function to search for the row and column that meet the specified criteria.
* Combine the two functions with multiplication and addition operations to create a dynamic search formula that can handle multiple criteria.

# Step 3: Applying Your Formula

Now that you understand the basics of the Index Match Multiple Criteria formula, it's time to put it into action. Here's an example scenario to help you get started:

Let's say you're managing a sales team and need to retrieve specific data about your sales reps based on their performance. You have a table with six columns: Name, Region, Sales, Units Sold, Commission %, and Commission Payment.

You want to create a formula that can search through the table and retrieve the Commission Payment for a specific sales rep based on the following two criteria:

* Sales Rep Name = "John"
* Region = "East"

To create your formula, you'd need to follow these steps:

1. Use the INDEX function to search within the table for the data you want to retrieve:

INDEX(range,

2. Use the MATCH function to search for the row that matches your first criteria (Sales Rep Name = "John"):

MATCH(1,(criteria1=range1),0))

3. Use the MATCH function again to search for the row that matches your second criteria (Region = "East"):

*(criteria2=range2),0))

4. Combine the two MATCH functions with multiplication and addition operations:

(MATCH(1,(criteria1=range1)*(criteria2=range2),0))

Putting it all together, your final formula should look like this:

INDEX(range,MATCH(1,(criteria1=range1)*(criteria2=range2),0))

# Conclusion

The Index Match Multiple Criteria technique is a powerful tool for searching through complex data sets and retrieving specific information based on multiple criteria. By combining the INDEX and MATCH functions, you can create a more flexible and dynamic search formula that can handle even the most complex data sets with ease.

We hope this article has provided you with the knowledge and resources you need to get started using this powerful Excel tool. With a little practice, you'll soon be revolutionizing your Excel skills and retrieving data with unmatched efficiency and accuracy!

{{< youtube 1lvHjivcjNc >}} 



## Index Match Multiple Criteria Rows and Columns
 
We all use the Excel VLOOKUP function day in and day out to fetch the data. Also, we know that the VLOOKUPVLOOKUPThe VLOOKUP excel function searches for a particular value and returns a corresponding match based on a unique identifier. A unique identifier is uniquely associated with all the records of the database. For instance, employee ID, student roll number, customer contact number, seller email address, etc., are unique identifiers.
read more function can bring the data from left to right, so the lookup value should always be on the left side of the result columns. However, we have several alternatives that can be used as an alternative to the VLOOKUP function in Excel. We can use these INDEX + MATCH formulaINDEX + MATCH FormulaThe INDEX function can return the result from the row number, and the MATCH function can give us the position of the lookup value in the array. This combination of the INDEX MATCH is beneficial in addressing a fundamental limitation of VLOOKUP.read more to match multiple criteria for rows and columns with advanced technology. So, this special article will take you through it in detail about this technique.
 
 You are free to use this image on you website, templates, etc.,  Please provide us with an attribution linkHow to Provide Attribution?Article Link to be HyperlinkedFor eg:Source: Index Match Multiple Criteria (wallstreetmojo.com) 
 
### How to Use INDEX + MATCH Formula to Match Multiple Criteria?
 
We explain using the INDEX+MATCH formula to match multiple criteria for rows and columns with examples.
 
#### Example #1 – INDEX + MATCH Formula
 
Not the majority of the Excel users lookup functions beyond the VLOOKUP. The reasons could be so many. Let us briefly introduce this formula before going to the advanced level.
 
For example, look at the below data structure in Excel.
 
We have “Sales Rep” names and their respective sales values. On the other hand, we have a drop-down list of “Sale Rep” in cell D2.
 
Based on our selection from the drop-down list “Sales” amount has to appear in cell E2.
 
We cannot apply the VLOOKUP formulaVLOOKUP FormulaThe VLOOKUP excel function searches for a particular value and returns a corresponding match based on a unique identifier. A unique identifier is uniquely associated with all the records of the database. For instance, employee ID, student roll number, customer contact number, seller email address, etc., are unique identifiers.
read more because the lookup value “Sales Rep” is to the right of the result column “Sales.” So in these cases, we can use the combination INDEX + MATCH lookup value formula.
 
The INDEX function looks for the mentioned row number value in the range A2:A11. Next, we need to provide from which row we need the sales value to come in this range. This row value is based on the “Sales Rep” name selected in the drop-down list in excelDrop-down List In ExcelA drop-down list in excel is a pre-defined list of inputs that allows users to select an option.read more, so the MATCH function looks for the “Sales Rep” row number in the range B2:B11 and returns the row number of the matched value.
 
#### Example #2 – Multiple Criteria in INDEX + MATCH Formula
 
Now, we have a data structure like the one below.
 
We have monthly sales values of “Sales Rep.” From this table, we need dynamic results like cell A15. So, we have created a “Sales Rep” drop-down list. In the B14 cell, we have created a “Month” drop-down list.
 
Based on the selection made in these two cells, our formula has to fetch the data from the above table.
 
For example, if we choose “Rep 8” and “Apr,” then it has to show the sales value of “Rep 8” for the month of “Apr.”
 
So, we need to match both rows and columns in these cases.
 
As we can see above, we have chosen “Rep 6” and “Apr” as the month, and our formula has returned the sales value for the month of “Apr” for “Rep 6”.
 
- We must first open the INDEX function in cell B15.  The first argument of the INDEX function is “Array,” i.e., from which range of cells we need the result. So, we need sales values in this case, so we must choose the range of cells from B2 to G11.  The next argument of the INDEX function is from which row of the selected range we need the result. In this case, we need to arrive at the “Sales Rep” row number based on the selection made in the cell A15 drop-down cell. So, we must open the MATCH function for dynamically fetching the row number based on our selection.  The lookup value of the MATCH function is “Sales Rep,” so we must choose the A15 cell as the reference.  The lookup array will be the “Sales Rep” named range in the main table. So, we must choose a range from A2 to A11.  The MATCH type of the MATCH function will be exact. So, we must insert zero as the argument value.  The next argument of the INDEX function is “Column Number,” i.e., from the selected range of cells from which column we need the result. It is dependent on the month we choose from the drop-down list of cell B14. So, to get the column number automatically, we must open another MATCH function.  The lookup value will be the month name, so select the B14 cell as the reference.  The lookup array will be the month range of cells in the main table, i.e., B1 to G1.  The last argument is MATCH type. Choose “Exact Match” as the criteria. Close two brackets and press the “Enter” key to get the result.

 

 
Note: Yellow-colored cell is the reference for you.
 
### Things to Remember
 
- Combining the Excel INDEX + MATCH function can be more powerful than the VLOOKUP formula.The INDEX and MATCH functions can match both rows and columnsRows And ColumnsA cell is the intersection of rows and columns. Rows and columns make the software that is called excel. The area of excel worksheet is divided into rows and columns and at any point in time, if we want to refer a particular location of this area, we need to refer a cell.read more headers and return the result from the middle table.The MATCH function can return the row number and column number of the table headers of both rows and columns.

 
### Recommended Articles
 
This article is a guide to Index Match Multiple Criteria. Here, we learn how to use the INDEX+MATCH formula to match multiple criteria in Excel and a downloadable Excel template. You may learn more about Excel from the following articles: –
 
- Excel Match Multiple CriteriaBreak-Even Analysis ExcelIndex Match in VBAVLOOKUP with Match in Excel




