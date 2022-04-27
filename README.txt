Samantha Creel & Michael Bottini
README file
From Canon to Fanfiction: Gender & Genre Trends

The TOOLS, DATASET, and ANALYSIS DATA used in this project can be found below, along with the link to the spreadsheets that contain our processed data that was used for analysis. 

TOOLS
Here we list the tools we used, which include (1) the fanfiction scraper tool to collect the fanfiction stories from fanfiction.net, (2) BookNLP to obtain the character mentions for each canon and story, (3) the iteration script so that BookNLP ran through every file in a given folder, rather than be manually commanded 312 times, and (4) the function to transform the BookNLP html output to a .txt file for import and analysis in Excel. Also included are the adjustments or additions needed for each tool to make our data collection more streamlined. Explanations for the adjustments can be found within the pages linked. 

(1) Fanfiction scraper tool: https://github.com/smilli/fanfiction
###
Adjustment to scraper tool (by Michael): https://drive.google.com/file/d/1aa4nQUEnutCpDY4D0mJuDGLVXS9mYPup/view?usp=sharing
Note:
GetFics Scraper: NoneType Error & Solution
GetFics ran fine for the first 50+ stories for me, but then I got the NoneType error for multiple lines relating to time. I think it's because FF.net changed the format of how they timestamp items since 2016, and so it messes with the code. I altered the original Scraper program to work around it.
So the altered Scraper file is in the Google Drive - To run the getfics function with the altered Scraper instead of the original, you need to move the altered file into the fanfiction directory, then re-name or delete the original file it came with.
###

(2) BookNLP: https://github.com/dbamman/book-nlp
(3) BookNLP Iteration (bash script) (by Michael): https://docs.google.com/document/d/18_5I9m2dYHLeTSR6TuesAQ8yLZ-4C4FhaBw7oieMADw/edit?usp=sharing
(4)  BookNLP html output to .txt file function for Jupyter Notebook (by Samantha):
BookNLP_2_Txt_Function.ipynb



DATASET
The dataset within this folder consists of the original .txt files of (5) all 12 canons and (6) all 300 fanfiction stories before processed through BookNLP, as well as the output, cleaned and converted (7) canon .txt counts and (8) story .txt counts after being processed through BookNLP.

There is one folder each for:
(5) Canon_txts -> Canon .txts
(6) Fanfiction_txts -> .txts (file names are numbered 1-25)
(7) Canon_BookNLP_txts --> Canon .txts BookNLP outputs
(8) Fanfiction_BookNLP_txts --> Fanfiction .txts BookNLP outputs
 

ANALYSIS DATA
We've included a link here to (9) our master spreadsheet containing all the data gathered after identifying the gender of each character and calculating their mention proportions. For Harry Potter, Lunar Chronicles, Phantom of the Opera, Peter Pan, Gone, and Chronicles of Narnia, the finalized version of each sheet can be viewed by going to Data > Filter Views > Gender M/F Final. The excel sheet that was used for analysis in R is also provided as number (10), as well as (11) the R markdown file.

(9) Master spreadsheet: 
	BookNLP Output Spread: https://drive.google.com/open?id=1i5d3owSIr8NZ2-iUJM8N6YboEDT6sd2Q1I6RYiWzkD4
(10) Master sheet for R with top ten characters: 
	CL Data: https://docs.google.com/spreadsheets/d/1fC7X-3edQeWDK3jHQXPHgG4dx5Lk3P0BfoZTJtVQie4/edit?usp=sharing
(11) R markdown file (Samantha): 
	Data_Analysis_Newplots.Rmd: https://drive.google.com/file/d/1gxpHPWexYObWxgbqLRogG94UrQQPFcaq/view?usp=sharing 
