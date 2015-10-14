# Early-warning-signals-of-financial-meltdowns

Written by Vishwesha Guttal, Centre for Ecological Sciences, Indian Institute of Science, Bangalore, 560012, India.

Edited and modified by Nikunj Goel, Undergraduate Department, Indian Institute of Science, Bangalore, 560012, India.

Install
1.	 R 
2.	 R Studio

Files
1.	main.R
2.	function_stock_analysis.R
3. 	dow jonex index per day data.csv
4. 	sp500 per day data.csv
5. 	nasdaq per day data.csv


Instruction to run the code

1. 	Load any of the three stock indexes. Command to load 	these data files is already in the the code in form of 	comments.

2. 	Insert a valid date in the code for which you want to 	calculate indicator trends. see 'stdcrashdate' in the 	code.

3. 	Click Source on the top right corner of the code window.

Common sources of error

1. 	All the files should be in the same folder.

2.	Set the working directory same as the folder in which 	all the files are present. Session/Set Working Directory/ 	To Source File Location.

3. 	Make sure before running the code you have installed all 	the required packages. 
	Required packages: a)moments b)Kendall c)KernSmooth.

4. 	Inserting a valid date is very important. Insert the date 	in dd/mm/yy format. see 'stdcrashdate' in the code.

		a) Data for DJI, SP500 and Nasdaq is only available 		   after 1896,1928 and 1971 respectively.

 		b) Make sure you do not enter a 	date which is not 		   present in the data files like weekends.

5.	Choose parameter values such that
	N > l_rw + l_ktau

6.	Choose parameter values such that 
	max(N_sensitivity) > max(rwrange) + max(l_kw) + 	max(k_end)

7.	The graph window might prompt "figure margins to large". 	In that case adjust the graph window for proper display.

Output

Output will consist of

1.	Kendall and pvalue table displayed in console window.

2.	Figure 3 equivalent of the main text in the graph window.
