---
title: "Attention Excel Users: Master the Art of Converting Text to Numbers with These 5 Proven Techniques!"
ShowToc: true 
date: "2022-12-03"
author: "Janice Malone"
---
*****
Attention Excel Users: Master the Art of Converting Text to Numbers with These 5 Proven Techniques!

As an Excel user, you know that one of the most common challenges in data analysis is working with numbers that are actually stored as text. This means that even if you use formulas that involve arithmetic operations, you might not get the results you expect. The good news is that there are several solutions to convert text to numbers in Excel, depending on the structure of your data and the desired outcome. Here are 5 proven techniques that can help you master this art and save time in your work.

1. Use the VALUE function

The simplest technique to convert text to numbers in Excel is to use the VALUE function. This function takes a text string as input and returns a numeric value that corresponds to that text, as long as it can be interpreted as a number. For example, if you have a cell that contains the text "123", you can use the formula =VALUE(A1) to convert it to the number 123. If the text contains non-numeric characters, such as commas, spaces, or currency symbols, you might need to remove them first with the SUBSTITUTE or TRIM function, as shown in the examples below:

=VALUE(SUBSTITUTE(A1,",",".")) - replaces commas with dots for decimal points
=VALUE(TRIM(SUBSTITUTE(A1,"$",""))) - removes dollar signs and trailing spaces

2. Use the Text to Columns feature

Sometimes, the text and numbers are mixed within the same cell or column, in a format that is not suitable for calculations. In this case, you can use the Text to Columns feature to split the data into separate cells or columns based on a delimiter or pattern. This feature is located under the Data tab, in the Text group, and allows you to specify the type of separator, such as comma, space, tab, or semicolon, and the destination cells for the converted text and numbers. By doing this, you can apply the VALUE function or other formulas to the numeric cells, and ignore or delete the text cells that are not needed.

To use the Text to Columns feature, select the column or range of cells that contains the mixed text and numbers, and then follow these steps:

- Click on the Text to Columns button
- Choose the Delimited option if the separator is a character, or Fixed Width if the data has a consistent pattern
- Select or type the separator character or positions for the split
- Preview the result in the Data Preview section
- Specify the format and location for the converted data, and click Finish

3. Use the Paste Special feature

Another technique to convert text to numbers in Excel is to use the Paste Special feature. This feature allows you to apply a specific operation or format to the data that you copy or cut from a source range, and paste into a destination range. If you have a whole column or range of cells that contains text that you want to convert to numbers, you can select that range, copy it, and then use the Paste Special option to apply the Multiply operation, which converts the text to numbers by multiplying each cell by 1. This works because Excel recognizes that multiplying a number by 1 does not change its value, but forces it to be treated as a numeric value.

To use the Paste Special feature with the Multiply operation, follow these steps:

- Copy the range of cells that contains the text you want to convert to numbers
- Select the destination range where you want to paste the converted data
- Right-click on the cell or range, and choose the Paste Special option
- In the Paste Special dialog box, select the Multiply option, and click OK
- The text should now be converted to numbers, without any loss of decimal places or formatting.

4. Use the Evaluate Formula feature

If you have a complex formula that involves text and numbers, and you want to see how Excel processes it step by step, you can use the Evaluate Formula feature. This feature allows you to view the current state of the formula, and each intermediate calculation, as you click on the Evaluate button. This can help you identify where the text values are interfering with the numeric values, and how to fix them. To access the Evaluate Formula feature, follow these steps:

- Select the cell that contains the formula you want to evaluate
- Click on the Formulas tab, and then click on the Evaluate Formula button
- Excel will highlight the next part of the formula that needs to be evaluated, and show its current value
- Click on the Evaluate button to see the result of that part, and then repeat for each step
- If you find a part that contains text instead of a number, you can use one of the previous techniques to convert it to a number, or modify the formula to exclude it.

5. Use the Find and Replace feature

If you have a large dataset that contains text that you want to convert to numbers, and you don't want to apply formulas or functions to each cell individually, you can use the Find and Replace feature. This feature allows you to search for a specific value or pattern in a range of cells, and replace it with another value or pattern, in one or more options, such as the entire workbook, or just a selected sheet or range. To use the Find and Replace feature for text-to-number conversion, follow these steps:

- Select the range of cells where you want to replace text with numbers
- Press Ctrl+H or go to the Home tab and click on the Find & Select button, then choose Replace
- In the Find what field, type the text value that you want to replace, or a pattern that matches several values
- In the Replace with field, type a numeric value that you want to replace it with, or leave it blank if you want to delete the text value
- Click on the Options button to specify additional search criteria, such as the search direction, whether to match case, or whether to search in formulas only
- Click on the Replace or Replace All button to apply the changes.

Conclusion

Converting text to numbers in Excel is a critical skill for data analysts and anyone who works with numerical data on a regular basis. By using at least one of these five proven techniques, you can save time, avoid errors, and get the results you need, without compromising the accuracy or integrity of your data. Whether you need to convert text to numbers for calculations, sorting, charting, or formatting purposes, Excel offers a variety of tools and features to make this process easy and effective.

{{< youtube QZxwsSJ3Za4 >}} 



One of the most common annoyances that people cite with Excel is dealing with how numbers and text are formatted in cells. It’s especially annoying when numbers inadvertently get entered into a spreadsheet in text format.
 
When this happens, calculations and different formulas don’t work quite right, or may not work at all. 
 
In this article you’ll learn how to identify when a column or row of numbers are actually formatted as text, and how to convert text to numbers so that they’ll work in formulas and calculations again. This is one of those basic Excel tips everyone should know. 
 

 
## Is Cell Data Text Or Numbers?
 
There are several ways you can see if a number or set of numbers in a column or row is formatted as text in Excel.
 
The easiest way is to select the cell, select the Home menu, and under the Number group in the ribbon, note the number format displayed in the dropdown box.
 
If the dropdown box displays “text”, you know the cell is formatted as text format. If you want to perform numerical calculations on the cell using Excel formulas, you’ll need to convert it first.
 
In the case where someone has entered numbers in text format using the apostrophe in the cell, you’ll see a small green triangle indicating the value has been entered as text.
 
Note: Preceding a cell entry with an apostrophe forces the cell formatting to text-based.
 
If you’ve discovered, using either of the approaches above, that the numerical data is entered into the Excel sheet in text format, you can use any of the methods below to convert that text to numbers.
 
## 1. Convert To Number
 
If you need to convert data that’s been entered into Excel with an apostrophe, you can easily convert it back to number format using the Convert to Number option.
 
1. First, select the cells you want to convert back to number format. You will see a yellow diamond appear near the selection with an exclamation symbol in the middle.
 
2. Select this symbol. From the dropdown, choose Convert to Number. 
 
This will update all of the text based numbers you’ve selected to the General numeric data format. 
 
You’ll know it worked when all the numbers in your selection switched from being left aligned to right aligned in the cells.
 
## 2. Using Text to Column
 
Another easy way to convert text to numbers in Excel is by converting over an entire column of values at once. You can do this using the Text to Column feature.
 
1. Select the entire column of data that you want to convert from text to numbers.
 
2. Select Data from the menu, and then select Text to Columns in the Data Tools section of the ribbon.
 
3. In the Wizard window, keep the default Delimited selected and select Next. 
 
4. On the next Wizard page, keep the default Tab selected, and select Next again.
 
5. Finally, on the last page of the Wizard, make sure General is selected under Column data format. For the Destination field, you can either select a new column where you want the number data to go, or just keep the current selected column as is. Select Finish.
 
Now your data will all be converted to numeric values, which you can use in Excel formulas and calculations.
 
Note: You’ll notice that the actual cell formatting doesn’t change from Text to General even though the values themselves can now be used as numbers. However, if you set your output column to a new column, you will notice that the formatting of the new column is set to General. This is only a cosmetic issue and doesn’t affect how the numbers in the “Text” formatted column behave.
 
## 3. Changing Cell Format
 
The easiest and fastest way to convert text to numbers in Excel is simply changing the cell formatting from the Home menu.
 
To do this:
 
1. Select all of the cells you want to convert. You can select an entire column (don’t include the header) if you want to convert all of the cells in a column.
 
2. Select the Home menu, and in the Number group on the ribbon, select the dropdown box with Text in it. 
 
3. You’ll see a list of formats to choose from. Select General to convert to number format. Or you can select Number, Currency, Accounting, or Percentage if you want those specific number formats applied to your numerical data.
 
## 4. Using Paste Values
 
If you need to move text cells that contain numbers into a new cell or column, you can use the Paste Special feature.
 
1. Select the group of empty cells where you want to place your output of numeric data. Select Format Cells from the pop-up menu.
 
2. In the window that opens, make sure General is selected as the number format and select OK.
 
3. Select the entire column of cells you want to convert from text to numbers, right-click, and select Copy.
 
4. Select the first cell in the empty column you formatted, right-click the cell and select Paste Values. You’ll see all of the text formatted numbers pasted in the General number format.
 
This works because when you select Paste Values, it pastes only the values from the source cell and not the original cell formatting. Instead, it uses the destination cell formatting, which you configured in the first part of this process.
 
## 5. Using The VALUE Function
 
There is a special function in Excel that’ll convert a number formatted as text into a numeric value. This is the VALUE function.
 
To use this function, select the cell where you want the converted number to go and type:
 
=VALUE(G2)
 
Replace “G2” above with the cell that has the number you want to convert. If you’re converting an entire column of numbers, start with the first cell only.
 
Press Enter and you’ll see that the text-formatted number has been converted to a General-format number. 
 
You can then fill the rest of the empty column to the bottom of that column and the VALUE formula will convert the rest of the cells in the original column as well.
 
After using any of these options for reformatting your numbers, you may need to refresh cell data after applying the new formatting. 
 
As you can see, there are a number of ways to convert text to numbers in Excel. The option you choose just depends on where you’re trying to place the output. It also depends whether you prefer using copy and paste, Excel formulas, or menu options.
 
Ultimately, each of these choices provides you with the same end result.



