---
title: "Unleashing the Hidden Power of Excel with the Ultimate Index Function: Master Examples, Formulas, and Step-by-Step Guide!"
ShowToc: true 
date: "2023-02-03"
author: "David Monske"
---
*****
# Unleashing the Hidden Power of Excel with the Ultimate Index Function: Master Examples, Formulas, and Step-by-Step Guide!

Microsoft Excel is a powerful tool that helps professionals across different domains to store, manage, analyze, and visualize data. Many people use Excel daily for their routine tasks like organizing customer data, creating invoices, and generating financial reports. However, Excel can do much more than that if you know how to harness its full potential.

One of the most important functions in Excel that you can use to work smarter and faster is the Index function. With the Index function, you can easily retrieve data from a table and arrange it in the way you want. In this article, we will show you how to unleash the hidden power of Excel with the Index function, and give you step-by-step guidance on how to use it.

## What is the Index function?

The Index function in Excel is a flexible formula that allows you to extract data from a table based on a specified column and row index. In simpler terms, it helps you find information in Excel worksheets and return the data that you need. The function is especially useful when you need to extract specific data from large tables or ranges.

The function has two major arguments: the array argument and the row and column index arguments. The array argument is the range of cells that contain the data you want to extract. The row and column index arguments refer to the position of the data you want to extract within the range.

## How to use the Index function

Now that you understand what the Index function is and what it does, it's time to learn how to use it. Here are the steps:

### Step 1: Open Excel and select the worksheet that contains the table or data range you want to extract information from.

### Step 2: Enter the Index function in the cell where you want the result to appear. The syntax of the Index function is as follows:

`=Index(Array,Row Number,Column Number)`

### Step 3: Enter the range or table you want to extract a value from in the Array argument.

### Step 4: Enter the row or column number in the Row and Column Number arguments for the cell you want to extract.

Once you have entered your Index formula, press Enter to see the extracted value or data.

## Index function examples

To give you a better understanding of how the Index function works, let's look at some examples:

### Example 1: Extracting a single value from a range

Let's say you have a range of data that contains customer names, addresses, and phone numbers. You want to extract the phone number of a specific customer, say John Smith. Here's how to do it:

1. Open Excel and select the worksheet that contains the customer data.
2. Enter the following Index formula in the cell where you want the phone number to appear:

`=Index(B2:D6, MATCH("John Smith",B2:B6,0), 3)`

In this formula, the Array argument is `B2:D6`, which is the range of cells containing the customer data. The Row Number argument is `MATCH("John Smith",B2:B6,0)`. This argument uses the Match function to find the row that contains the specific customer name you want to extract, which is "John Smith" in this example. The Column Number argument is `3`, which corresponds to the phone number column.

### Example 2: Extracting multiple values from a table

Let's say you have a table that contains sales data for different products in different regions. You want to extract the sales data for a specific region, say Europe, and put the results in a separate table. Here's how to do it:

1. Open Excel and select the worksheet that contains the sales data.
2. Create a new table or range where you want to extract the data.
3. Enter the following Index formula in the cell where you want the first extracted value to appear:

`=Index(A2:H13, SMALL(IF($D$2=$F$2:$F$13, ROW($F$2:$F$13)-MIN(ROW($F$2:$F$13))+1,""),ROW()-ROW($E$2)+1),COLUMN()-COLUMN($F$2)+1)`

In this formula, the Array argument is `A2:H13`, which is the range of cells containing the sales data. The Row Number argument uses the Small function to extract the row numbers of the cells that match the specified criteria, which is `$D$2=$F$2:$F$13`. This argument looks for the cells in the F column that match the value in D2, which is "Europe" in this example. The Column Number argument uses the Column function to extract the column numbers of the cells in the range.

## Conclusion

The Index function is a powerful tool that you can use to extract and organize data in Excel worksheets. By mastering the function, you can save time and effort and work smarter. We hope that this article has provided you with a better understanding of the Index function and how to use it, and has helped you unleash the hidden power of Excel.

{{< youtube lrkwwNGfbKU >}} 



## Index Function in Excel
 
The INDEX function in Excel helps extract the value of a cell, which is within a specified array (range) and, at the intersection of the stated row and column numbers. In other words, the function goes to the cell (within a particular range) whose position is specified, picks its value, and returns it as the output. The INDEX function can also extract an array of values from a dataset.
 
For example, a worksheet contains the names of continents and the corresponding countries. The entries, typed in Excel (without the double quotation marks), are listed as follows:
 
Column A
 
- Cell A1 contains “Asia.”Cell A2 contains “Africa.”Cell A3 contains “Europe.”Cell A4 contains “North America.”

 
Column B
 
- Cell B1 contains “India.”Cell B2 contains “Nigeria.”Cell B3 contains “France.”Cell B4 contains “Canada.”

 
Enter the formula “=INDEX(A1:B4,3,2)” in cell C1. Press the “Enter” key and the output is “France” (without the double quotation marks).
 
First, the INDEX excel function goes to the range A1:B4. From this range, it fetches the value of the cell, which is at the intersection of the third row (row 3) and the second column (column B). This cell is B3 and its value is “France.”
 
The INDEX function can return the following values:
 
- The value at the intersection of the specified row and column numbersThe value within a table or a named range whose row and column numbers are specifiedThe value within non-adjacent ranges whose row and column numbers are specified

 
The INDEX function in Excel is useful when the dataset is large and one knows the position of the cell from which the value needs to be extracted.
 
The INDEX function is categorized under the Lookup and Reference functions of Excel.
 
 You are free to use this image on you website, templates, etc.,  Please provide us with an attribution linkHow to Provide Attribution?Article Link to be HyperlinkedFor eg:Source: INDEX Function in Excel (wallstreetmojo.com) 
 
### Syntax of the INDEX Function in Excel
 
There are two forms of the INDEX function in excel, the array and the reference. The syntax of both forms is shown in the following image.
 
Let us discuss both forms of the Excel INDEX function one by one.
 
The Array Form of the INDEX Excel Function
 
In the array form, the INDEX function fetches the value of a cell within an array or a table. An array can be either a single range of cells (horizontal or vertical) or multiple adjacent ranges. The value of the cell, which is at the intersection of the supplied row and column numbers, is returned.
 
The INDEX function accepts the following arguments in the array form:
 
- Array: This can be a range of cells, table, array constant or named rangeNamed RangeName range in Excel is a name given to a range for the future reference. To name a range, first select the range of data and then insert a table to the range, then put a name to the range from the name box on the left-hand side of the window.read more. The cell whose value is to be returned must necessarily be within this array.Row_num: This is the row number of the array from which the value is to be returned.Column_num: This is the column number of the array from which the value is to be returned.

 
The arguments “array” and “row_num” are mandatory, while the argument “column_num” is optional.
 
It is essential to specify either the “row_num” or the “column_num” to extract a value from a one-dimensional array. To extract a value from a two-dimensional array, one needs to specify both, the “row_num” and the “column_num.”
 
Note 1: A one-dimensional array consists of a single row or a single column. A two-dimensional array consists of multiple rows and columns.
 
Note 2: If both “row_num” and “column_num” are entered as zeros (or blanks), the “#VALUE!” error is returned. For instance, the formulas “=INDEX(A1:A4,0,0)” and “=INDEX(A1:A4,,)” return the “#VALUE!” error.
 
Note 3: If the “array” argument consists of a single column, the “column_num” argument can be omitted, but the “row_num” must be supplied to fetch the value. Likewise, if the “array” argument consists of a single row, the “row_num” argument can be omitted, but the “column_num” must be specified to fetch the value.
 
For instance, in case of a single column, use the formula “=INDEX(array,row_num)” to fetch a value. In case of a single row, use the formula “=INDEX(array,,column_num)” to fetch a value.
 
The Reference Form of the INDEX Excel Function
 
In the reference form, the INDEX function fetches the value of a cell within a defined area (array or range). There can be multiple non-adjacent areas in the reference form. In such cases, the particular area, within which the INDEX function should look for the value, can be specified.
 
The INDEX function in Excel accepts the following arguments in the reference form:
 
- Reference: This is the area which can either be a single range or multiple non-adjacent ranges. In the case of multiple non-adjacent ranges, use commas to separate the ranges. In addition, all the ranges must be enclosed within parentheses. For instance, the “reference” argument, (A1:C2, C4:D7) implies two areas (arrays or ranges), A1:C2 and C4:D7.Row_num: This is the row number of the area from which the value is to be returned.Column_num: This is the column number of the area from which the value is to be returned.Area_num: This number indicates the area (of the “reference” argument) in which the INDEX function will look for a value. The first area of the “reference” argument is assigned the number 1. The second area is numbered 2 and so on. For instance, if the “reference” argument is (A1:C2, C4:D7, F4:H8) and the “area_num” is 3, the INDEX function looks for the value in the third area of the “reference” argument, i.e., F4:H8.

 
The arguments “reference” and “row_num” are required, while the arguments “column_num” and “area_num” are optional.
 
In the following image, the grey box (pointed by the red arrow) shows the different areas (arrays or ranges) of the reference argument. Further, the area numbers of each range are also given.
 
Note 1: If the “area_num” argument is omitted, the INDEX excel function looks for the value in the first area of the “reference” argument.
 
Note 2: All the areas stated in the “reference” argument should be located on one worksheet. If the first area is in one worksheet and the second is in another, the INDEX function returns the “#VALUE!” error.
 
Note 3: The difference between the array and reference forms is that in the former, adjacent ranges are used, while in the latter, non-adjacent ranges are used.
 
### How to use the INDEX Function in Excel?
 
Let us consider a few examples to understand the working of the INDEX function in Excel.
 
#### Example #1–Array Form With a One-Dimensional Array
 
The following image shows the number of employees (column C) working in the different departments (column B) of an organization.
 
We want to extract the value of cell C7 with the help of the INDEX function. Use the array form with column C as the single array.
 
The steps to perform the given task are listed as follows:
 
Step 1: Enter the following formula in cell E2.
 
“=INDEX(C3:C7,5)”
 
Step 2: Press the “Enter” key. The output in cell E2 is 4.
 
Explanation: In the formula entered in step 1, we omitted the “column_num” argument since the array (C3:C7) is a single column. Cell C7 is in the fifth row of the array C3:C7. So, the “row_num” argument is entered as 5.
 
Hence, the given INDEX formula returns 4, which is the value of row 5 of the range C3:C7.
 
#### Example #2–Array Form With a Two-Dimensional Array
 
The following image shows the total number of employees working in five departments of a multinational corporationMultinational CorporationA multinational company (MNC) is defined as a business entity that operates in its country of origin and also has a branch abroad. The headquarter usually remains in one country, controlling and coordinating all the international branches.
read more (MNC). The numbers pertain to four years, namely, 2015-2018.
 
We want to extract the value of cell E5 with the help of the INDEX excel function. Use the array form with the entire dataset (except the headings in row 2) as the array.
 
Step 1: Enter the following formula in cell B9.
 
“=INDEX(B3:F7,3,4)”
 
Step 2: Press the “Enter” key. The output in cell B9 is 629.
 
Explanation: In the preceding formula (entered in step 1), the multiple rows and columns of the dataset are entered as a single array (B3:F7). The INDEX formula returns the value of the cell, which is at the intersection of row 3 and column 4 of the range B3:F7. The cell at this position is cell E5 and its value is 629.
 
Hence, the output, 629, corresponds to the third row and fourth column of the range B3:F7.
 
#### Example #3–Array Form With Row and/or Column Numbers as Zeros
 
Working on the data of example #2, we want to apply the INDEX function to the entire dataset (B3:F7). Further, observe the output in the following cases:
 
Case 1: When both arguments “row_num” and “column_num” are zeros
 
Case 2: When either the “row_num” or the “column_num” is zero
 
The two cases are discussed as follows:
 
Case 1: When both row and column numbers are entered as zeros, the INDEX function returns the “#VALUE” error.
 
Steps to be followed: Enter the formula “=INDEX(B3:F7,0,0)” in cell B9. Press the “Enter” key and the output is the “#VALUE” error. This is shown in the following image.
 
Conclusion: When multiple rows and columns are used as an array, it is necessary to specify both the row and column numbers to extract a particular cell value. In case, both row and column numbers are entered as zeros, the output is the “#VALUE” error.
 
Case 2: When either the row or the column number is zero, and the INDEX formula is entered as an array formula, the output is an array of values.
 
Steps to be followed: Select the blank range B11:B15. Enter the formula “=INDEX(B3:F7,0,1)” in the first cell selected (cell B11). Press the keys “Ctrl+Shift+Enter” together.
 
The outputs in cells B11, B12, B13, B14, and B15 are “Sales,” “HR,” “Operation,” “Marketing,” and “Finance” respectively. All outputs are obtained (without the double quotation marks) the way they are displayed in the range B3:B7.
 
Alternatively, select the blank row D11:H11. Enter the formula “=INDEX(B3:F7,3,0)” as an array formula. The output is the array of values of row 5 (of the preceding image). So, the output is “Operation,” “176,” “665,” “629,” and “497” without the double quotation marks.
 
Conclusion: When either the row or column number is specified while the other is set at zero, the INDEX function returns an array of values. However, in such cases, the INDEX formula must be entered as an array formula.
 
Moreover, it is essential to select a blank output range prior to entering the INDEX formula. This output range should have as many blank cells as the array of the source dataset.
 
Note: An array formula is usually completed by pressing the CSE keys (Ctrl+Shift+Enter).
 
#### Example #4–Reference Form With Multiple Two-Dimensional Arrays
 
The following image contains three datasets which display the number of employees working in the different departments of an MNC. The first dataset (B2:E7) shows the figures for the years 2015-2017. The second (D9:F12) and third datasets (C14:E18) show the figures for the years 2015 and 2016.
 
Use the reference form of the INDEX excel function to extract the value of cell F11. Further, categorize the three datasets into three areas which exclude the top row containing the headings.
 
The steps to perform the preceding tasks are listed as follows:
 
Step 1: Enter the following formula in cell B20.
 
“=INDEX((B3:E7,D10:F12,C15:E18),2,3,2)”
 
Step 2: Press the “Enter” key. The output is 665, as shown in the following image.
 
Explanation: In the preceding formula (entered in step 1), the three datasets (given in the question of this example) have been categorized into three areas of the “reference” argument. These areas are B3:E7, D10:F12, and C15:E18. The headings have been excluded from these areas.
 
Further, the INDEX function looks for a value in the second area (D10:F12). This is because the “area_num” argument is 2. The arguments “row_num” and “column_num” are 2 and 3 respectively. So, the INDEX function returns the value of the cell, which is at the intersection of the second row and the third column in the area D10:F12. This is cell F11.
 
Hence, the output of the INDEX formula is 665.
 
### The Properties Applicable to Both Forms of the INDEX Function
 
The properties applicable to both the array and reference forms are listed as follows:
 
a. If both the arguments “row_num” and “column_num” are entered as zeros, the INDEX excel function returns the “#VALUE!” error.
 
b. To fetch a value from a single column array, use the following formulas:
 
- “=INDEX(array,row_num)” in the array form“=INDEX((reference),row_num,,area_num)” in the reference form

 
To fetch a value from a single row array, use the following formulas:
 
- “=INDEX(array,,column_num)” in the array form“=INDEX((reference),,col_num,area_num)” in the reference form

 
c. If all the column values of an array are required vertically, specify the “column_num” and set the “row_num” at zero. Likewise, if all the row values of an array are required horizontally, specify the “row_num” and set the “column_num” at zero. In both cases, select a blank output range prior to entering the INDEX formula. Moreover, press the keys “Ctrl+Shift+Enter” to complete the formula.
 
d. The arguments “row_num,” “column_num,” and “area_num” should refer to a cell within the defined array or reference. If not, the INDEX function returns the “#REF!” error.
 
Note: In pointer “c,” the blank output range can be selected vertically or horizontally depending on whether a vertical or a horizontal array is required.
 
Further, the number of blank cells (of the output range) must be equal to the cells of the particular row or column array (which is being copied) of the source dataset.
 
### The INDEX With Other Functions of Excel
 
The INDEX function in excel can be used with several other functions of Excel in the following ways:
 
a. The INDEX function is used in combination with functions like SUM, AVERAGE, MIN, and MAX to create dynamic ranges. For instance, the formula “AVERAGE(C3:INDEX(C3:C7,3))” returns the average of cells C3, C4, and C5. This is because the formula “INDEX(C3:C7,3)” returns a reference to cell C5. So, the resulting formula becomes “AVERAGE(C3:C5).” Moreover, with a change in the “row_num” argument of the INDEX function, the range of the AVERAGE function changes. This results in a change in the output obtained.
 
b. The INDEX and MATCH MATCH Function In ExcelThe MATCH function looks for a specific value and returns its relative position in a given range of cells. The output is the first position found for the given value. Being a lookup and reference function, it works for both an exact and approximate match. For example, if the range A11:A15 consists of the numbers 2, 9, 8, 14, 32, the formula “MATCH(8,A11:A15,0)” returns 3. This is because the number 8 is at the third position.
read more functions are used together to perform left lookups. This combination of the INDEX and MATCH functions overcomes the limitations of the VLOOKUP function of Excel. For instance, limitations like compulsory sorting of data, restricted size of the lookup value, decreased speed of Excel, and so on are eliminated.
 
c. The INDEX function can be used with the COUNTA functionCOUNTA FunctionThe COUNTA function is an inbuilt statistical excel function that counts the number of non-blank cells (not empty) in a cell range or the cell reference. For example, cells A1 and A3 contain values but, cell A2 is empty. The formula “=COUNTA(A1,A2,A3)” returns 2.
read more to extract the value of the last used cell of a dataset. With a change in the value of the last used cell, the output updates on its own.
 
Note 1: Dynamic ranges automatically update with the addition or deletion of data.
 
Note 2: Usually, the INDEX function returns the value of a cell. However, when a cell referenceCell ReferenceCell reference in excel is referring the other cells to a cell to use its values or properties. For instance, if we have data in cell A2 and want to use that in cell A1, use =A2 in cell A1, and this will copy the A2 value in A1.read more and colon (:) precede the INDEX function, it returns a cell reference. This can be observed in the AVERAGE and INDEX formula of pointer “a.” 
 
### Frequently Asked Questions
 
### Recommended Articles
 
This has been a guide to the INDEX function in Excel. Here we discuss the working of the INDEX formula in Excel along with examples and a downloadable Excel template. You may also look at these useful functions in Excel–
 
The INDEX function in Excel returns the value of a cell whose array has been defined. In addition, the row and column numbers of this cell are also specified in the arguments of the INDEX formula. The INDEX function can also retrieve the values of the entire row or column of a range. The INDEX function has two versions, the array and the reference. Both versions have their own set of arguments. Note: For details related to the arguments of the INDEX function, refer to the heading “the syntax of the INDEX function in Excel” of this article.
 
The steps for using the INDEX function in Excel are listed as follows: a. Select the relevant form (array or reference) of the INDEX function to be applied. For this, take into consideration the kind of data. b. Supply the arguments to the INDEX function. If an array of values is required, select a blank output range prior to entering the arguments. c. Press either the “Enter” key or the CSE (Ctrl+Shift+Enter) keys, depending on the kind of output required. The INDEX function processes the arguments. Next, it returns either a single value or an array of values based on the way it has been used.
 
The INDEX MATCH functions are a versatile combination. This is because these functions can easily lookup a value, regardless of the location of the lookup and the return columns. The formula to perform a lookup (in rows and columns) by using the INDEX MATCH functions is stated as follows: “=INDEX(column to return a value from,MATCH(vlookup value,column to be looked up,0),MATCH(hlookup value,row to be looked up,0))” The working of this formula is explained as follows: a. The formula “MATCH(vlookup value,column to be looked up,0)” looks for the vlookup value in the column to be looked up (or lookup column). This formula looks for the exact match and returns the row number. b. The formula “MATCH(hlookup value,row to be looked up,0)” looks for the hlookup value in the row to be looked up (or lookup row). This formula looks for the exact match and returns the column number. c. The INDEX function uses the row and column numbers returned by the MATCH function. The INDEX function returns a corresponding value from the “column to return a value from” (or return column). Hence, the INDEX and MATCH formula returns a value at the intersection of certain row and column numbers. Note 1: It is also possible to supply only the row number or only the column number to the INDEX function. For supplying only the row number, use the first MATCH formula (given in pointer “a”) with the INDEX function. Likewise, to supply only the column number, use the second MATCH formula (given in pointer “b”) with the INDEX function. Note 2: Looking for a value at the intersection of a row and column is called a 2-way lookup (or 2-dimensional lookup or matrix lookup).
 
- VLOOKUPINDIRECT in ExcelPOWER Function in excelHyperlink Excel | Examples




