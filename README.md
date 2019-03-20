# Hack the Border, NEW 508, March 20, 2019

Step 1: Download the zip file at https://data.transportation.gov/Research-and-Statistics/Border-Crossing-Entry-Data/keg4-3bc2/data. Note that this file was downloaded from Data downloaded from https://data.transportation.gov/Research-and-Statistics/Border-Crossing-Entry-Data/keg4-3bc2/data on March 20, 2019, and included all variables for all years and saved as a CSV. 

Step 2: Move to desktop and uncompress/extract  

Step 3: Let's now examine this csv using the command line and then open it in excel 

From Mac:
Type "terminal" in Spotlight to launch
"change directory" -> cd ~/desktop
List files -> LS
head Border_Crossing_Data.CSV
open -a "Microsoft Excel" Border_Crossing_Entry_Data.csv
More on CVS from the Mac Terminal at https://bconnelly.net/posts/working_with_csvs_on_the_command_line/

From Windows 10: 
Cortina Search -> PowerShell 
"change directory" -> cd desktop
List files -> dir 
gc .\Border_Crossing_Entry_Data.csv | select -first 10
Invoke-Item .\Border_Crossing_Entry_Data.csv

Step 4: Parse the location variable. {  =clean(a:a) -> paste values only -> text to columns -> find and replace }

Step 5: Create a discrete year variable with insert, filter and fill 

Step 6: Create a variety of pivot tables to generate findings. Which border has more crossings? What specific port is the busiest? How do the ports in NY compare? What considerations do we need to give considering the nature of the "measures" variable? 

Step 7: Save a series of individual csv files of things you might want to try to visualize. 

