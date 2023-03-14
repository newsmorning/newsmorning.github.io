---
title: "Revolutionize Your Excel Skills with the Ultimate Vlookup Hack - Discover the Game-Changing Index Match Function Today!"
ShowToc: true 
date: "2023-05-03"
author: "Laurel Scroggins"
---
*****
# Revolutionize Your Excel Skills with the Ultimate Vlookup Hack - Discover the Game-Changing Index Match Function Today!

Are you tired of struggling with Excel's VLOOKUP function? Do you find yourself constantly searching for a better solution to lookup and retrieve data from large tables? Look no further than the INDEX MATCH function to revolutionize your Excel skills.

VLOOKUP has long been a go-to function for looking up values in a table based on a specific input. However, it has limitations that can make it difficult to use in certain situations. One major drawback is that it can only look up values to the right of the matching column. This limitation can make it difficult to work with tables that have data arranged in a non-standard way.

Enter the INDEX MATCH function. This versatile function can overcome the limitations of VLOOKUP and provide a more flexible solution for looking up data. The function is made up of two components: INDEX and MATCH.

The INDEX function allows you to specify a range of cells and return the value of a particular cell within that range. The MATCH function searches for a specified value in a range of cells and returns the relative position of that value within the range.

By combining the two functions, you can create a lookup formula that can search for a value in any column of a table and return the corresponding value from a different column. This approach allows for more flexible data lookup, regardless of the arrangement of data in the table.

Here's how to use the INDEX MATCH function in Excel:

1. Identify the range of cells in the table that contains the data you want to retrieve.

2. Use MATCH function to find the position of the lookup value within the column you want to search.

3. Use INDEX function to return the corresponding value from the desired column.

The syntax for the function looks like this: =INDEX(column to retrieve value from, MATCH(lookup value, column to search, 0))

The "match_type" argument is set to 0 to ensure that an exact match is found. If a match cannot be found, the function will return an error value.

So, now you may be wondering, why should you switch to INDEX MATCH? Here are a few reasons:

1. Flexibility: Unlike VLOOKUP, INDEX MATCH can return a value from any column within the table, not just to the right of the matched column.

2. Non-exact lookups: With VLOOKUP, you can only do exact matches. With INDEX MATCH, you can do partial matches or even fuzzy matches.

3. Efficiency: INDEX MATCH uses fewer resources than VLOOKUP, making it a faster and more optimized solution for large data sets.

In conclusion, the INDEX MATCH function is a game-changing tool that can help you take your Excel skills to the next level. It overcomes the limitations of VLOOKUP and provides a more flexible, efficient, and customizable solution for data lookup. If you are serious about using Excel for data analysis or any other work, mastering INDEX MATCH should be at the top of your list.

{{< youtube yH_ArqoB0no >}} 



## What Does INDEX Function Do in Excel?
 
The INDEX function can return the result from the row number. In addition, the MATCH function can give us the lookup value position in the array. The combination of the INDEX MATCH Excel function is very useful in addressing a key limitation of VLOOKUP, which we cannot use to search the table from left to right. However, the INDEX MATCH function can achieve this goal effortlessly. In this article, we will discuss this in detail.
 
For example, suppose we have an Excel worksheet containing the list of student’s names and the corresponding scores they achieved in the exams in the range A1:B4. If we need to extract the value of cell A1 which contains the student name, “Micheal,” which is within the specified array (range), we can use the INDEX function. Using the INDEX function,“=INDEX(A1:B4,1,1),” we can obtain the required extracted values at the intersection of the specified row and column numbers. In this scenario, inserting the INDEX Excel function formula in cell C1, it reaches the range A1:B4. And fetches the cell’s value at the intersection of the first row (row 1) and the first column (column A). The cell is A1, and its value is “Micheal.” So, the Excel INDEX function returns “Micheal.”
 
In the same Excel worksheet, suppose we need to know the position of the scores ( score is 80, which is in column B1) achieved by the student, “Micheal” Therefore, in such a scenario, we can use the Excel MATCH function. Applying the MATCH formula, “MATCH(80,A11:A15,0),” returns 1 since the score achieved by Micheal is at the first position in the Excel worksheet. 
 
It is as simple as that. For now, look at the syntax of the INDEX function.
 
Array: From which column or array do we need the value?
 
Row Number: In the provided array, do we need the result from which row?
 
These two arguments are good enough in most situations. So, now we will look into the example of the INDEX function.
 
### Example
 
For this example, consider the below data.
 
We have data from A1 to B7 cell range. In the D2 cell, we have the month name, and for this month’s name, we need sales value in cell E2.
 
Let us open the INDEX function in cell E2.
 
An array is the first argument, i.e., from which column we need the result, i.e., we need results from the “sales” column, so select from B2 to B7.
 
Next is the ROW number, i.e., the selected range of cells from which row we need the result. In this example, we need the sales value for the month “Mar.” In the selected range, “Mar” is the third row, so we need results from the third row.
 
Ok, that’s all. Close the bracket and press the “Enter” key. We will have sales value for the month of “Mar.”
 
Like this, based on the row number provided, we will get the value from the supplied array.
 
### What Does MATCH Function Do in Excel?
 
The MATCH function is used to find the lookup value position in the supplied array. In simple terms, lookup value row number or column number in the range of cells. Below is the syntax of the MATCH functionSyntax Of The MATCH FunctionThe MATCH function looks for a specific value and returns its relative position in a given range of cells. The output is the first position found for the given value. Being a lookup and reference function, it works for both an exact and approximate match. For example, if the range A11:A15 consists of the numbers 2, 9, 8, 14, 32, the formula “MATCH(8,A11:A15,0)” returns 3. This is because the number 8 is at the third position.
read more.
 
Lookup Value: For which lookup value are we trying to find the position?
 
Lookup Array: In which array or range of cells are we looking for the lookup value?
 
Match Type: This will decide what kind of result we need. We can provide zero for an exact match.
 
#### Example of MATCH Function in Excel
 
For this example, consider the above data only.
 
From the above data, we are trying to get the month “Mar” position in cell E5. So, we must open the MATCH function in the E5 cell.
 
The first argument is “lookup value,” so here, our lookup value is “Mar,” therefore, select the D5 cell.
 
The lookup array is from which range of cells we are trying to look for the lookup value position. So, we must select the “Month” column.
 
The last argument is “MATCH type” since we look at the exact match supply 0.
 
So, in the lookup array A2:A7, the position of the lookup value “Mar” is 3.
 
### Combination of INDEX + MATCH Function in Excel
 
The INDEX can return the result from the mentioned row number, and the MATCH function can give us the position of the lookup value in the array. Instead of supplying the row number to the INDEX formula, we can enclose the MATCH function to return the row number.
 
We must first open the INDEX function in cell E2.
 
For the first argument, the array supplies B2 to B7.
 
Instead of supplying the row number as 3, open the MATCH function inside the INDEX function for the row number.
 
Select the lookup value as a D2 cell.
 
Now, we must select the lookup array as A2 to A7.
 
Then, we must insert zero as the match type.
 
So, based on the row number provided by the MATCH function, the INDEX function will return the sales value. We can change the “Month” name in cell D2 to see dynamically changing sales value.
 
### Powerful Alternative to VLOOKUP
 
We all have used the VLOOKUP functionVLOOKUP FunctionThe VLOOKUP excel function searches for a particular value and returns a corresponding match based on a unique identifier. A unique identifier is uniquely associated with all the records of the database. For instance, employee ID, student roll number, customer contact number, seller email address, etc., are unique identifiers.
read more day in and day out. But, one of the limitations of VLOOKUP is that it can only fetch the value from left to right, not from right to left.
 
For example, look at the below data.
 
#### 
 
The above data lookup value is “Month,” and the result column is “Sales.” But, the data result column (Sales) is to the left of the lookup array table (Month), so we cannot use the Excel VLOOKUP function here, but we can still fetch with the combination of the INDEX function with the MATCH function for the data from the table.
 
### Recommended Articles
 
This article is a guide to Index Match Function in Excel. Here, we learn how to use the INDEX and MATCH functions as a powerful alternative to VLOOKUP along with examples and a downloadable Excel template. You may learn more about Excel from the following articles:
 
- Index Match With Multiple CriteriaVenn Diagram ExamplesCreate Box and Whisker Plot ExcelVBA Index Match




