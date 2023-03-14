---
title: "Discover the Secret Excel Function That Will Revolutionize Your Spreadsheets!"
ShowToc: true 
date: "2023-02-07"
author: "Lee Boyd"
---
*****
# Discover the Secret Excel Function That Will Revolutionize Your Spreadsheets!

Are you tired of manually formatting your spreadsheets, spending countless hours trying to get your data to look presentable? Fortunately, Excel has a secret function that can quickly transform your spreadsheet game. The magic function is called Conditional Formatting, and it will transform the way you look at spreadsheets forever.

Conditional Formatting is a function within Excel that allows you to format cells based on specific conditions or rules. With this function, you can highlight data that meets certain criteria, such as thresholds or ranges. This can help you easily identify important data points or trends within your spreadsheet, without having to manually go through each cell and apply formatting manually.

Let's say you have a spreadsheet that tracks sales data for your business over the last few months. You want to quickly identify which months had the highest sales and which ones had the lowest. With Conditional Formatting, you can automatically highlight the highest and lowest sales months in seconds. Here's how:

1. Select the column containing the sales data.

2. Click on Conditional Formatting in the Home tab of the ribbon menu.

3. Choose "Highlight Cell Rules" and then "Top/Bottom Rules".

4. Choose "Top 10 Items".

5. Choose a formatting style for the top 10 items.

6. Repeat for the bottom 10 items.

Voila! Your spreadsheet will now highlight the top and bottom 10 sales months, allowing you to easily identify the most important data points.

But Conditional Formatting can be used for much more than just highlighting data. You can also use it to format cells based on particular values, such as dates, text, or numbers. This is especially useful when working with large sets of data, as you can quickly identify patterns or trends without having to spend hours manually formatting.

To get started with Conditional Formatting, try experimenting with different rules and formatting options. You'll soon discover just how powerful this function can be and how much time it can save you in the long run.

In conclusion, if you want to take your spreadsheet game to the next level, look no further than Conditional Formatting. This secret Excel function can revolutionize the way you work with data and allow you to make better, data-driven decisions. So what are you waiting for? Give it a try today and see how it can transform your spreadsheets!

{{< youtube Qi1nfN5F8F4 >}} 



## INDIRECT Function In Excel
 
The INDIRECT Excel function indirectly refers to cells, cell ranges, worksheets, and workbooks. First, it accepts a text string entered as an argument and converts it into a valid cell address. Next, it goes to this cell address and returns its value.
 
For example, in the next image, cell B1 contains the text string “c4.” Enter the formula “=INDIRECT(B1)” in any cell, e.g., D7. This INDIRECT Excel formula works as follows:
 
- The INDIRECT function refers to cell B1, which consists of “c4.”The INDIRECT function goes to cell C4 and returns its value “Jessica” in cell D7.

 
In this way, the text string “c4” is converted into the cell address C4. Then, the INDIRECT Excel function heads to this cell address (C4) and returns its value (Jessica).
 
The INDIRECT function lets the user specify an indirect cell address in the form of a text string. Apart from cells, this function can also refer to named ranges, other workbooks, and worksheets with the help of text strings.
 
The advantage of using the INDIRECT Excel function is that the indirect references do not change with the insertion or deletion of new rows or columns. Moreover, the user can change the text string (indirect cell address) of the cell referred to in the formula without changing the INDIRECT formula itself.
 
For instance, in the preceding example, type “c2” (without the double quotation marks) in cell B1 and retain the formula “=INDIRECT(B1).” So, this time the INDIRECT function goes to cell C2 and returns its content. Hence, the text string changed rather than the INDIRECT Excel formula.
 
Using the INDIRECT Excel function converts text values into valid cell addresses. The INDIRECT function is categorized under the LOOKUP and REFERENCE functions of Excel.
 
### Syntax of the INDIRECT Function
 
The syntax of the INDIRECT function of Excel is shown in the following image:
 
The function accepts the following arguments:
 
- ref_text: This is a cell address or cell referenceCell ReferenceCell reference in excel is referring the other cells to a cell to use its values or properties. For instance, if we have data in cell A2 and want to use that in cell A1, use =A2 in cell A1, and this will copy the A2 value in A1.read more. It refers to the cell which contains a text string. This text string is an indirect cell address that we can specify in either the A1-style or the R1C1-style. “Ref_text” can also refer to a cell containing the name of a named range, a workbook, or a worksheet.a1: This is a logical (or Boolean) value–true or false. It specifies the style of reference used by the “ref_text” argument. It can take either of the following values:

 
The argument “ref_text” is mandatory while “a1” is optional.
 
Note 1: If the text string is entered in R1C1-style reference (like r2c3), it is compulsory to enter the “a1” argument (as 0 or false) in the INDIRECT excel formula.
 
Note 2: For more on A1-style and R1C1-style references, refer to the topic “how is the A1-style different from the R1C1-style of referencing?” at the end of example #5.
 
### How to Use the INDIRECT Function in Excel?
 
Let us consider a few examples to understand the working of the INDIRECT function in Excel.
 
#### Example #1–Reference to a Named Range
 
The following table displays the number of visitors to the website www.xyz.com. These visitors have been categorized under different channels. Each channel is listed in the column “Search Channel.”
 
Further, these visitors belong to five countries: India, the USA, Australia, Singapore, and Canada. Each country is represented by its respective column.
 
We want to perform the following tasks:
 
The steps to perform the given tasks are listed as follows:
 
Step 1: In row 8, we must calculate the total visitors of each country by applying the SUM function. The totals of columns B, C, D, E, and F are shown in the next image.
 
Create a named range for the data of each country. Let us begin by naming the range F3:F7 as “Canada.” For this, perform the following tasks:
 
a. Select the range F3:F7.
 
b. In the name box, type “Canada” without the double quotation marks. The name box is to the left of the formula bar and is shown with a red arrow in the next image.
 
c. Press the “Enter” key.
 
The range F3:F7 has been named “Canada.”
 
Note: The names of the named ranges are not case-sensitive. It implies that if a range is called “figures,” the terms “FigUres,” “fIguReS,” etc. mean the same to Excel.
 
The alternative method to create a named range has been discussed in the following pointers (step 1a to step 1c).
 
Step 1a: Select the range (F3:F7) to be named.
 
- Click “Name Manager” from the “Formulas” tab of the Excel ribbon.Click “New.”

 
Step 1b: The “New Name” box opens. Next, perform the following tasks:
 
a. In the “Name” box, type “Canada” without the double quotation marks.
 
b. In “Refers to,” the selected range F3:F7 is displayed. If this range is not showing in the “Refers to” box, select it.
 
c. Click “OK.” Finally, close the “Name Manager” dialog box.
 
The selected range (F3:F7) has been named “Canada.” The selection of this range has been shown in the following image and the image under step 1a.
 
Step 1c: Likewise, we must create named ranges for the numbers of all the five countries. The five named ranges titled Australia (D3:D7), Canada (F3:F7), India (B3:B7), Singapore (E3:E7), and USA (C3:C7) have been created.
 
The named ranges are shown in the following image.
 
Step 2: To calculate the total number of visitors from Canada, enter the following formula in cell I4.
 
“=SUM(INDIRECT(H4))”
 
The INDIRECT Excel function refers to cell H4, which contains the name “Canada.” It goes to the range “Canada” (F3:F7) and returns its total. That is because the INDIRECT function is enclosed within the SUM function.
 
Step 3: Before applying the data validation feature, a named range consisting of the names of the five countries needs to be created. For this, perform the following tasks in the given sequence:
 
a. Select “Name Manager” from the “Formulas” tab and click “New.” The “New Name” dialog box opens.
 
b. In the “Name” box, type “Country” (without the double quotation marks), as shown in the following image.
 
c. In the “Refers to” box, select the cells B2:F2. Click “Ok.”
 
d. Close the “Name Manager” window.
 
A named range titled “Country” is created.
 
Step 4: Apply the data validationData ValidationThe data validation in excel helps control the kind of input entered by a user in the worksheet.read more feature to cell H4. For this, perform the following tasks in the stated order:
 
a. Select the cell (H4) to which we must apply the data validation feature.
 
b. Click the “Data Validation” drop-down from Excel’s “Data” tab. Select “Data Validation.”
 
c. The “Data Validation” window opens, as shown in the following image. In the “Settings” tab, select “List” from the “Allow” drop-down.
 
d. In “Source,” type “=Country” without the double quotation marks.
 
e. Select “Ignore blank” and “In-cell drop-down ” checkboxes.” Click “OK.”
 
The data validation feature has been applied to cell H4. Therefore, depending on whether the checkbox of “in-cell dropdown” is selected or not (in step d), a drop-down arrow may or may not appear next to cell H4.
 
The drop-down arrow does appear next to cell H4, though it has not been shown in the following images. This drop-down arrow (next to cell H4) shows the names of the five countries, India, USA, Australia, Singapore, and Canada.
 
Note: The data validation feature restricts the input that a user can enter in a cell of a worksheet. It allows the user to enter only those values defined by the data validation rule.
 
Step 5: Once the data validation feature has been applied, we must enter the name of any of the five countries (India, USA, Australia, Singapore, and Canada) in cell H4. The total number of visitors to the selected country will appear in cell I4.
 
To insert the name of a country in cell H4, one can either type the required country or select it from the drop-down arrow next to cell H4.
 
An error message appears if an input other than the names of the given five countries is entered in cell H4. This message states that restrictions have been defined for this cell (H4).
 
For instance, enter “India” in cell H4. The sum of its visitors (30,019) appears in cell I4. It is shown in the following image.
 
In the following pointers (step 5a to step 5b), the results of the data validation feature are examined.
 
Step 5a: Enter “Australia” in cell H4. The total number of visitors (30,336) appears in cell I4. The same is shown in the following image.
 
Step 5b: Enter “Australia” in cell H4. The total number of visitors (30,336) appears in cell I4. The same is shown in the following image.
 
Hence, one must note that we did not change the INDIRECT Excel formula of cell I4 to obtain the total visitors of the different countries. We only changed the names of the ranges in cell H4.
 
Thus, we changed the cell’s content referred to in the formula (H4) without changing the formula itself (in cell I4).
 
#### Example #2–Reference to a Worksheet
 
The next images (image 1, image 2, and image 3) show the sales revenue (in $) generated by the different channels (under “Search Channel”) in other countries. Every channel represents a category of visitors to the website www.xyz.com.
 
Further, one image has been created in one Excel worksheet. As a result, every worksheet has been named by the country it represents. So, for instance, the worksheet containing the numbers of India has been called “India.”
 
The total sales revenue of five countries (India, USA, Australia, Singapore, and Canada) has been shared. These totals have been calculated with the SUM function of Excel.
 
- Calculate the total sales revenue generated by each country using the INDIRECT and the SUM functions.Cross-check the results of the INDIRECT function in excel (enclosed within SUM) with the simple SUM function.

 
The total sales revenue of Singapore and Canada are $65,358 and $20,600, respectively. For these countries, assume that the sales generated by the different channels are listed in the range C2:C8 of the worksheets titled “Singapore” and “Canada,” respectively. Cell C2 contains the caption “Sales,” and cell C8 has the sum of the range C3:C7 (calculated by the SUM function).
 
[Please note that the total sales revenues calculated with the SUM function have been shared to enable cross-checking of results.]
 
Image 1
 
The total sales revenueSales RevenueSales revenue refers to the income generated by any business entity by selling its goods or providing its services during the normal course of its operations. It is reported annually, quarterly or monthly as the case may be in the business entity's income statement/profit & loss account.read more (in $) of India is shown in the following image:
 
[Consider the entire column “search channel” as range B2:B8 of the worksheet “India.” The column “sales” is in the range C2:C8. These ranges also include the titles of the green boxes.]
 
Image 2
 
The total sales revenue (in $) of the USA is shown in the following image:
 
[Consider the column “search channel” as range B2:B8 of the worksheet “USA.” The column “sales” is in the range C2:C8.]
 
Image 3
 
The total sales revenue (in $) of Australia is shown in the following image:
 
[Consider this image as a part of the worksheet titled “Australia.”]
 
The steps to calculate the total sales revenue of the different countries by using the INDIRECT Excel function are listed as follows:
 
Step 1: To find the total sales revenue generated by each country, concatenate (join) the name of the worksheet and the channel-wise sales figures (listed in the “sales” column of the preceding images). It is because the sales figures of different countries are in separate worksheets.
 
In cell C4, begin typing the following INDIRECT Excel formula.
 
“=SUM(INDIRECT(B4”
 
The same is shown in the next image.
 
Step 2: Complete the preceding formula (entered in step 1) in cell C4.
 
“=SUM(INDIRECT(B4&”!C3:C7))”
 
The same is shown in the following image.
 
The “ref_text” argument (B4&”!C3:C7) begins with cell B4, which contains “India.” “India” is the name of the worksheet which contains image 1. So, in the first argument of the INDIRECT function, we refer to the worksheet indirectly by its name.
 
Further, we use the operator ampersand (&) for combining the sheet name (India) in cell B4 and the range to be summed up (C3:C7) in image 1.
 
Step 3: Press the “Enter” key. The output appears in cell C4, as shown in the following image.
 
Since the INDIRECT function in excel is enclosed within the SUM function (refer to the formula entered in step 2), the sum of the range C3:C7 of worksheet “India” is returned.
 
Hence, the total revenue of $199,363 matches the “SUM” amount of image 1. It implies that the result of the preceding formula (in step 2) is the same as that of the simple SUM function (in the second succeeding image).
 
The application of the SUM function to the range C3:C7 has been shown in the following image to allow cross-checking of results.
 
In the following pointers (step 3a to step 3c), the total sales revenue of the different countries is examined.
 
Step 3a: For calculating the total sales revenue of the USA, perform the following tasks:
 
- Enter “USA” (without the double quotation marks) in cell B4.Enter the formula “=SUM(INDIRECT(B4&”!C3:C7))” in cell C4.Press the “Enter” key.

 
In the given INDIRECT Excel formula, the value of cell B4 (worksheet named “USA”) is joined with the range (C3:C7 of image 2) to be summed.
 
Hence, the total revenue of $1,030,984 appears in cell C4. This number is the same as the “sum” amount of image 2.
 
Step 3b:  Enter “Singapore” in cell B4. The formula to be entered in cell C4 remains the same as in the preceding step (step 3a).
 
Press the “Enter” key. The output of $65,358 appears in cell C4, as shown in the following image.
 
Step 3c:  Enter “Canada” in cell B4. Retain the same formula as the preceding step (step 3a).
 
The output in cell C4 is $20,600.
 
Likewise, we can calculate the total sales revenue of Australia by entering the respective name in cell B4 and retaining the formula of cell C4.
 
Hence, by changing the sheet names (in cell B4) and retaining the formula (in cell C4), we have obtained the total sales revenue of the different countries. Please note that we made no changes to the INDIRECT formula (in cell C4).
 
Thus, we changed the values of the first argument, “ref_text” (different sheet names), though the cell address of the INDIRECT excel formula remains the same (B4).
 
#### Example #3–Reference to the Last Month (R1C1-Style)
 
The next images (image 1, image 2, and image 3) show the sales revenue (in $) generated by the different channels (under “search channel”) in the first three months of 2018. The entire data relates to the website www.xyz.com.
 
- Find out the total sales revenue of the last month (March) by using the R1C1 reference style of the INDIRECT function in excel.Add a fifth column (column E) to the existing dataset, which contains the sales of April. Find out the total sales revenue of the last added month (April) by using the R1C1-style of the INDIRECT function.Cross-check the output of the INDIRECT formulas with the totals of the respective months. These totals have been calculated with the help of the SUM function of Excel.

 
The figures of April are–$12,943 (organic search), $7,279 (direct visitor), $7,889 (paid search), $10,327 (social visitors), $2,154 (referral), and $40,592 (total).
 
The channel-wise sales revenues (in $) for January, February, and March are shown in the following image:
 
The total sales revenue ($) for January, February, and March are shown in the following image:
 
The total sales revenues of March and April are to be calculated in the cell B13 (containing a question mark) shown in the following image:
 
Step 1: Begin by entering the following formula in cell B13.
 
“=INDIRECT(“R10C”&COUNTA(10:10))”
 
Step 2: Complete the preceding formula (step 1) in cell B13.
 
“=INDIRECT(“R10C”&COUNTA(10:10),FALSE)”
 
The first argument of the INDIRECT excel function is “R10C”&COUNTA(10:10). In this argument, we have concatenated R10C and the COUNTA functionCOUNTA FunctionThe COUNTA function is an inbuilt statistical excel function that counts the number of non-blank cells (not empty) in a cell range or the cell reference. For example, cells A1 and A3 contain values but, cell A2 is empty. The formula “=COUNTA(A1,A2,A3)” returns 2.
read more with the help of the operator “&.” The COUNTA function counts the total number of non-empty cells in row 10. It returns 4.
 
So, R10C joined with 4 results in the cell number R10C4. Since the second argument of the INDIRECT function is “FALSE,” R10C4 is recognized as an R1C1-style reference by Excel.
 
Note: For more on R1C1-style references, refer to the topic “how is the A1-style different from the R1C1-style of referencing?” at the end of example #5.
 
Step 3: Press the “Enter” key. Since the “ref_text” argument evaluates to R10C4, the INDIRECT Excel formula returns the cell value at the intersection of row 10 and column 4. In the A1-style, this is cell D10 of Excel.
 
Hence, the output is $249,344.
 
Step 4: Add the sales figures for April in column E of the existing dataset. Enter the following formula in cell B13.
 
The first argument of the INDIRECT Excel function is “R10C”&COUNTA(10:10), and the second argument is “FALSE”. The COUNTA function returns the value 5 as there are five non-empty cells in row 10.
 
When R10C is joined with 5, it results in R10C5. This R10C5 is the R1C1-style reference which implies cell E10 (A1-style). The row number is 10, and the column number is 5 (column E).
 
Hence, the INDIRECT Excel formula returns the value of cell E10. So, the total sales revenue for April is $40,592.
 
Likewise, we can add the sales data for the remaining months to the existing dataset. Then, with the same INDIRECT formula (entered in steps 2 and 4), we can obtain the total sales revenues of the last added month.
 
One can notice that even after adding the data for April, the INDIRECT Excel formula remained the same. In other words, the INDIRECT formula we used for calculating the sales revenue for March is the same as that of April.
 
The INDIRECT formula did not change because it perceives “R10C” in the “ref_text” argument as a text string.
 
Hence, the indirect references do not change with the insertion or deletion of new rows or columns in Excel.
 
#### Example #4–Reference to a Table Array
 
The following image contains five table arrays. Each array includes the sales revenue generated from the different visitor channels (under “search channel”) of a website (www.xyz.com).
 
One table array represents the data of one country. For the five countries, India, USA, Canada, Australia, and Singapore, the table arrays are named “Ind,” “States,” “Can,” “Aus,” and “Sin,” respectively.
 
In addition, the entire range of every table array is a named range. The name of the range is the same as the name of the table array. For instance, the range D2:E7 has been called “Ind,” G2:H7 has been named “States,” and so on.
 
- Obtain the sales of the “Direct Visitor” channel of Singapore (in cell B3) with the help of the VLOOKUP functionVLOOKUP FunctionThe VLOOKUP excel function searches for a particular value and returns a corresponding match based on a unique identifier. A unique identifier is uniquely associated with all the records of the database. For instance, employee ID, student roll number, customer contact number, seller email address, etc., are unique identifiers.
 - read more of Excel.Obtain the sales of Singapore’s “Direct Visitor” channel (in cell B3) by using a combination of the VLOOKUP and INDIRECT functions.Obtain the sales of India’s “Referral” channel (in cell B3) by using a combination of the VLOOKUP and INDIRECT Excel functions.

 
One can cross-check the output of the preceding pointers with the figures of the respective table arrays.
 
Step 1: To obtain the sales of the “Direct Visitor” channel of Singapore by the VLOOKUP function, perform the following tasks:
 
a. Enter “direct visitor” (without the double quotation marks) in cell B1.
 
b. Ensure that the range G10:H15 is named “Sin.” Thereafter, enter “Sin” in cell B2.
 
c. Enter the formula “=VLOOKUP(B1,B2,2,0)” in cell B3.
 
d. Press the “Enter” key.
 
The output “N/A” error appears in cell B3, as shown in the following image.
 
The “N/A” error appears because we have mistakenly entered the “table_array” argument (second argument) as “B2.” Unfortunately, the VLOOKUP function could not recognize this argument (B2). The “table_array” argument is always entered as a range of cells.
 
Hence, an incorrect argument makes the VLOOKUP formula return an error.
 
Had we entered the VLOOKUP formula as: “=VLOOKUP(B1,G10:H15,2,0)” in cell B3, the output would have been $4,587.
 
Step 2: To obtain the sales of the “Direct Visitor” channel of Singapore by a combination of the VLOOKUP and INDIRECT functions, perform the following tasks:
 
- Enter “Direct Visitor” in cell B1 and “Sin” in cell B2. The range G10:H15 has already been named “Sin” in the preceding step (step 1).Enter the formula “=VLOOKUP(B1,INDIRECT(B2),2,0)” in cell B3, as shown in the following image.

 
The first argument, cell B1 is the “lookup_value” of the VLOOKUP function. So, this function searches for the string “Direct Visitor.”
 
The INDIRECT excel function refers to cell B2, which contains “Sin.” This “Sin” is the “table_array” argument of the VLOOKUP function. The VLOOKUP function searches for the string “direct visitor” in the range “Sin” (G10:H15).
 
Further, the “col_index_num” argument is 2. So, the VLOOKUP function searches for the lookup value (direct visitor) in the second column of the range “Sin.”
 
Since the fourth argument (range_lookup) is 0, the given VLOOKUP formula returns an exact match. An exact match is a value equal to the lookup value.
 
Step 3: Press the “Enter” key. The output of $4,587 appears in cell B3. This output matches the value of cell H12 which is a part of the table array of Singapore.
 
Hence, the preceding formula (entered in step 2) has returned the sales of Singapore’s “Direct Visitor” channel.
 
Step 4: To obtain the sales of the “Referral” channel of India with the help of the VLOOKUP and INDIRECT functions, perform the following tasks in the stated order:
 
- Enter “referral” in cell B1 and “Ind” in cell B2.Ensure that the range D2:E7 is named “Ind.”Enter the formula “=VLOOKUP(B1,INDIRECT(B2),2,0)” in cell B3.Press the “Enter” key.

 
The output appears in cell B3, as shown in the succeeding image.
 
We have changed the values of cells B1 and B2 to “Referral” and “Ind,” respectively. Since named ranges are not case-sensitive, “IND” and “Ind” mean the same to Excel.
 
The first argument (lookup_value) of the VLOOKUP is “B1.” The output of “INDIRECT(B2)” works as the “table_array” argument of the VLOOKUP function. The “col_index_num” argument is 2. The “range_lookup” argument is 0 or false (exact match).
 
The VLOOKUP searches for the value “referral” in the named range “Ind” (D2:E7). It returns an exact match from the second column of the range “Ind.”
 
Hence, India’s “Referral” channel sales are $3,192. This output does match with the value of cell E7. This cell is a part of the table array of the country India.
 
Likewise, we can change the values of cells B1 and B2 to obtain the different sales numbers in cell B3.
 
We must note that the formulas entered in steps 2 and 4 are the same. Therefore, retain this formula to obtain the required sales figures in cell B3. Next, we must change the values of cells B1 and B2 according to the output required in cell B3.
 
#### Example #5–Reference to a Drop-down List
 
The following image shows three designations (director, manager, and supervisor) prevalent in an organization. These positions (designations or ranks) are listed in column A. Columns C, D, and E state the names of those employees who are currently serving in these positions.
 
- Create a drop-down list in cell I2. When the drop-down arrow is clicked, the list must display the names of the three positions (Director, Manager, and Supervisor).Create a dependent drop-down list in cell I3. As a position is typed in cell I2, the corresponding names of employees (serving at that position) should be displayed. For instance, if “Director” is typed in cell I2, cell I3 should show the names of the Directors (listed in column C) of the organization.

 
Use the named ranges, data validation feature, and the INDIRECT function of Excel.
 
Step 1: Name the ranges of the given dataset. For naming the ranges, select the range and type the required name in the name box (refer to step 1 of example #1).
 
The ranges should be named as follows:
 
- Name the range A2:A4 as “Position.”Name the range C2:C3 as “Director.”Name the range D2:D5 as “Manager.”Name the range E2:E7 as “Supervisor.”

 
Note:While naming the ranges, do not enter the beginning and the ending double quotation marks (shown in the preceding pointers) in the name box.
 
Step 2: For creating a drop-down list in cell I2, perform the following steps:
 
- Select cell I2. Click the “Data Validation” drop-down from the “Data” tab of Excel. Select “Data Validation.”In the settings tab of the “Data Validation” window, select “List” under the “Allow” drop-down.Under “Source,” Type “Position” (without the double quotation marks).Select the checkboxes of “ignore blank” and “in-cell dropdown.”

 
A drop-down list is created in cell I2, as shown in the following image. When the drop-down arrow (next to cell I2) is clicked, the names of the three positions (director, manager, and supervisor) appear.
 
To enter a position in cell I2, one can either type it or select it from the drop-down list.
 
Step 3: To create a dependent drop-down list in cell I3, we need to apply the data validation feature to the given cell. For this, perform the following steps:
 
Select cell I3. Click the “Data Validation” drop-down from the “Data” tab of the Excel ribbon.
 
b. Select “Data Validation.” The “Data Validation” window opens.
 
c. In the “Settings” tab, select “List” under “Allow.”
 
d. Select the checkboxes of “Ignore blank” and “In-cell dropdown” if they are not selected.
 
e. Under “Source,” enter the formula “=INDIRECT($I$2)” without the double quotation marks. Click “OK.”
 
The same is shown in the following image. Once “OK” is clicked (in step e), the drop-down arrow appears in cell I3.
 
In the following pointers (step 3a to step 3c), the different drop-down lists (in cell I3) that appear on typing the position (in cell I2) have been examined.
 
Step 3a: Type “Director” (without the double quotation marks) in cell I2. Clicking the drop-down arrow of cell I3 displays the names of employees, Andrew and Micheal. These employees are serving in the mentioned position.
 
Step 3b: Type “Manager” (without the double quotation marks) in cell I2. The drop-down of cell I3 displays the names Camille, David, Davis, and William. These employees are the managers of the organization.
 
Step 3c: Type “Supervisor” (without the double quotation marks) in cell I2. The drop-down of cell I3 displays the names of the employees working as supervisors in the organization: Alex, Diana, Sam, Austin, Shawn, and John.
 
We must note that the drop-down list of cell I3 is dependent on cell I2. Therefore, it implies that cell I3 displays the names of employees corresponding to the name of the position typed in cell I2.
 
Before creating a dependent drop-down list (in cell I3), ensure that all ranges (in columns A, C, D, and E) are named and after that, apply the data validation feature to cell I3.
 
### How is the A1-Style Different From the R1C1-Style of Referencing?
 
In the A1-style of referencing, every cell address consists of a column letter followed by a row number. For instance, address C5 refers to the cell at the intersection of column C and row 5.
 
In the A1-style referencing, every cell address consists of a column letter followed by a row number. For instance, address C5 refers to the cell at the intersection of column C and row 5.
 
On the other hand, in the R1C1-style, a cell address consists of a row number followed by a column number. Instead of letters, every column has a unique number assigned to it. For instance, cell A2 in A1-style is called R2C1 in R1C1-style.
 
To change the Excel reference style from A1 to R1C1, perform the following steps:
 
- From the File tab of Excel, click “options.”The “Excel Options” window opens. Select “Formulas.”Under “Working with formulas,” select the checkbox of “R1C1 reference style.”Click “OK.”

 
Consequently, all the column letters will change to numbers. Moreover, if there are any formulas in the worksheet, their cell references will adjust according to the R1C1-style.
 
### The Cautions While Working With the INDIRECT Excel Function
 
The cautions to be observed while working with the INDIRECT function of Excel are listed as follows:
 
- The “ref_text” argument must be a valid cell reference. If not, the INDIRECT function will return the “#REF!” error.The “ref_text” argument can refer to another workbook (an external reference). Ensure that the concerned workbook (source workbook) is open. If not, the INDIRECT function will return the “#REF!” error.The “ref_text” argument must not refer to a cell range beyond the maximum of 1,048,576 rows or 16,384 columns (XFD). The INDIRECT function in excel returns a “#REF!” error if it does.

 
The “#REF!” error is shown in the following image.
 
Note: In the modern versions of Excel, XFD is the right-most column of a worksheet.
 
### Frequently Asked Questions
 
### Recommended Articles
 
This article is a guide to the INDIRECT Excel function. Here we discuss how to use an INDIRECT formula in Excel and step-by-step examples. Take a look at the following articles in Excel: –
 
The INDIRECT function returns the value of a cell whose address is provided by a text string. In other words, the function can interpret text strings as valid cell addresses (or cell references). Once analyzed, the function goes to this cell address, picks its value, and returns it.The INDIRECT function does not perform any calculations. It just evaluates a reference and displays its content. The text string (or the reference) entered in the function can be changed without changing the INDIRECT formula.The syntax of the INDIRECT function of Excel is stated as follows:“INDIRECT(ref_text,[a1])”The “ref_text” argument is the cell address that contains a text string, a named range, or the name of a worksheet or workbook.The “a1” argument is the value true or false. If “a1” is true or 1 (or omitted), the “ref_text” argument is treated as an A1-style reference. If “a1” is false or 0, the “ref_text” argument is considered in R1C1-style.
 
With the help of the INDIRECT function and the data validation feature, it is possible to create dependent drop-down lists. A dependent drop-down list displays a series of items depending on selecting a value in another cell.For example, there are two lists titled “flowers” and “trees” in an Excel worksheet. First, let us create a dependent drop-down list in cell E3. This list should be dependent on the value entered in cell E2.The text “flowers” is displayed in cell A1. This list contains the following items:• Cell A2 contains Rose • Cell A3 contains Lotus • Cell A4 contains Sunflower • Cell A5 contains Tulip The text “trees” is shown in cell B1. This list contains the following items:• Cell B2 contains Oak • Cell B3 contains Pine • Cell B4 contains Maple • Cell B5 contains Spruce The steps to create a drop-down list in cell E3, which depends on cell E2, are listed as follows:a. Name the range A2:A5 as “Flowers” and B2:B5 as “Trees.”b. Select cell E3.c. Click the “Data Validation” drop-down from the “Data” tab of Excel. Select “Data Validation.”d. In the “Settings” tab, select “List” under the “Allow” drop-down.e. Under the “Source” drop-down, enter the formula “=INDIRECT($E$2).” The list (of cell E3) should depend on the value selected in cell E2.f. Select the two checkboxes of “Ignore blank” and “In-cell dropdown.” Click “OK.”A dependent drop-down list is created in cell E3.When “Flowers” is typed in cell E2, the drop-down arrow next to E3 displays the list–Rose, Lotus, Sunflower, and Tulip. Similarly, if “Trees” is typed in cell E2, cell E3 shows the Oak, Pine, Maple, and Spruce values.Note: Please do not enter the double quotation marks in the name of the range (in step a) and the INDIRECT Excel formula (in step d).
 
We should use the INDIRECT function of Excel for the following reasons:a. It helps indirectly refer to a cell, range, worksheet, or workbook.b. It allows fixing a reference to not change with the insertion or deletion of rows or columns.c. It helps obtain different outputs by changing the text string to which the INDIRECT formula refers.We should use the INDIRECT function of Excel in the following situations:a. It is used when there is a need to create dynamic cell references. For making a dynamic reference to a range, enter its name in a cell, and refer to that cell in the INDIRECT formula [like “=INDIRECT(C1)” where the cell C1 contains the name of the range].b. It is used when there is a need to convert a text string into a valid cell address. The text string supplied to the function can be changed as per the user requirement without changing the actual INDIRECT formula.c. It is used when there is a need to lock a cell reference. A cell reference is locked to prevent it from changing with the insertion or deletion of rows or columns. For instance, the formula “=INDIRECT(“B2”)” identifies “B2” as a text string rather than a cell reference. The string “B2” remains intact with the insertion of a row preceding cell B2 (like row 1).
 
- Indirect Labor ExampleExcel Check MarkExcel Indirect FormulaName Manager in Excel




