# ABC
Automated Bibtex Capitalization ABC. This project is to develop a set of codes that statisticians may use the program to automagically enforce capitalization within their bibtex files that are copied from the google scholar bibtex outputs.  


To get bibtex entries for your bib files from google scholar navigate to www.google.com/scholar navigate to settings ear the top center of the window. One of the last options allows you to set the import specifications to bibtex. 
Select this option and click save. Now you will be able to select entries for bibtex from your query output and copy and save the bibtex entry into a central .bib file. This file has a flaw for the entries copied from google scholar. 
These entries will not contain  braces "{ }" around capital letters in the title field. These capital letter will not be displayed as capitals without these braces. 

This project attempts to solve this problem within the field of statistics and perhaps, math, physics, computer science, IE/OR and affiliated fields. Certainly the best coverage is from my own background, statistics. Others interested in expanding this
project to establish better coverage results on various related domains of study. 

Fork requests and collaborations are highly encouraged. I'm happy to share the work on this with other and to specialize to fields of specialization. 

to invoke this project after download at the command line: 

sed -nf  bibfix test_case1.bib | less 

where you may replace test_case1.bib with the path to the file you want to run the correcton codes on and the bibfix file  which contains all of the regex code fixes. Only lines that are edited based on the code will be displayed in the output. Note this does not store the results into another file. To store the output in a different file so you still maintain the original copy before the changes from the script, type: 

sed -f  bibfix test_case1.bib > output_file_name 

where output_file_name is the file you want to store the output file.
