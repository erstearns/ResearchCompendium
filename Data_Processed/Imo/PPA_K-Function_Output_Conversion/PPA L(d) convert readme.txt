Readme for PPA L(d) and L*(d) conversion.
Roberto Cortinas
cortinas@uiuc.edu
June 20, 2003

This Excel file is meant to automate the task of taking K-function (second-order analysis) (routine #4) and weighted K-function (routine #5) PPA outputs into Excel for assessment of significance and development of graphs.

The workbook has six sheets:

1. PPA_K_output
2. Formulas
3. L(d)
4. Chart L(d)
5. L'(d) - (only for weighted K)
6. Chart L'(d) - (only for weighted K)

Instructions:

1. Import or paste the PPA K or weighted-K output into the PPA_K_output sheet. Select the PPA_K_output sheet. (IMPORTANT: Make sure that PPA_K_output is the current sheet and that the data is imported into A1, the uppermost and left cell). When instructed to convert the text into columns, select Delimited. Go to next page and select SPACE delimiter. Keep the "Treat consecutive delimiters as one" checked. You can uncheck the TAB delimiter. Press the FINISH button. Put the data into the existing worksheet. 

2. In the Formulas sheet you will see some basic information derived from the PPA output. In the top rows I wanted to check the furthest X and Y distance between points and to calculate the area. I have noticed differences between the area derived by multiplying these maximum distances and the area calculated in PPA. Check to see that the number of points, max search distance, step size, and steps are all correct.

3. The L(d) and L'(d) sheets should only display their corresponding outputs. You can copy and paste special the values onto a new worksheet (don't copy the formulas or else you will only create a relative worksheet). I have not tried just saving the worksheet in another format that only saves the sheet values (e.g. dbf).

4. The chart worksheets probably may not formatted correctly for your data - that's because they are set up for 10 intervals. To improve the graphs' appearance, follow the instructions on the L(d) and L'(d) sheets on how to change the maximum row ranges for all graph values and x-axis labels. Once you do this, the graphs should look fine.
Save the graphs as other worksheets.

Loading the next output:

When importing the next PPA output, it is NOT necessary to clear the PPA_K_output sheet (if the number of intervals is the different among outputs, you will have to modify the graphs). Just make sure that you use the command REFRESH DATA.

Toolbar / Data / Refresh Data
OR
Right-click in A1 and select Refresh Data from the drop-down menu.

However, if you want to make sure that there are no problems, you can clear the PPA_K_sheet prior to importing the new output.

1. To reuse the worksheet run the macro that automatically clears the columns.
Press ALT-F8 and RUN the macro!
USE THIS OPTION. IT'S THE EASIEST AND LESS ERROR PRONE.

2. Other ways to clear columns:

a. close without saving and reopen (will have to redo graph range corrections);
b. clear columns A through H on the PPA_K_output sheet (do not delete otherwise the remining worksheets will lose the reference to the first sheet!!).

********* For Excel 2002 (Office XP) *********

1. Select columns A through H on the PPA_K_output sheet.
2. Do either of the following steps:
	i. Go to Toolbar / Edit / Clear / Contents
	ii. Right-click highlighted columns -> select "clear contents"
3. You will then get a message asking if you want to delete the query as well as the cell contents. SELECT NO.

Now you can import more PPA K or weighted-K outputs
1. Either...
	i. Go to Toolbar / Data / Refresh Data
	ii. Right-click on worksheet and select "Refresh Data"
2. If a filename appears in the File Name section, Clear the name and more files should appear. If the outputs do not have *.txt extensions, select "All Files" for file type.
3. Import data. In most cases, the imported output file will be automatically formatted into columns!
4. If the intervals / steps are the same, you will probably NOT have to modify the graph ranges!
**********************************************

2. Specs:

MAX STEPS: 100

More intervals could be analyzed, but requires copy and pasting the formulas in several worksheets. Additionally, more memory would be required and the file will get even larger.

3. Changing graph formats

Make sure that if you change the formatting to suit your tastes, save the file without any imported data!

____________________________________________
This file is FREEWARE. Use of this file is AT YOUR RISK.
THIS FILE IS NOT MADE, DISTRIBUTED, OR SUPPORTED BY THE UNIVERSITY OF ILLINOIS AT URBANA-CHAMPAIGN, SAN DIEGO STATE UNIVERSITY, DONGMEI CHEN OR ARTHUR GETIS.

Point Pattern Analysis (PPA) Version 1.0
DongMei Chen and Arthur Getis, SDSU, CA.