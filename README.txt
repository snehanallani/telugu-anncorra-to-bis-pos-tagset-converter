TAGSET CONVERTER TOOL

README

Dependencies : 
1. Python - argparse module (Usually distributed with default python version)

Folder Structure : 
-------------------------------------------------------------------------------------------------------------------------
<File/Folder>					<Description>
extract.py					Source Code.
argumentParser.py				File to parse the command-line arguments given with the main code.
map.xml						Contains the TAG mapping rules. Can be changed.(Default argumen to -m)
wordList					A sample folder containing Word-Lists for BIS TAGS.
wordList/BIS_wordList				Folder that contains the BIS\_Tagset Word-Lists.(Default argument to -w))
wordList/Other_wordList			        Folder to put Word-Lists for other Tagsets.
dataset						Folder with sample Files for conversion.
dataset/test_input				Folder with sample Input Files.(Default argument to -i)
dataset/test_output				Folder with sample Output Files.(Default argument to -o)
-------------------------------------------------------------------------------------------------------------------------

How to Use : 
1. To convert from ILMT Tagset to BIS Tagset : 

   >> ./extract.py -i inputDatasetFolder -o outputDatasetFolder -m map.xml -w wordlist/BIS_wordlist/
   
   where inputDatasetFolder is the folder with all the SSF format files that are to be converted.
   	 outputDatasetFolder is the folder where the files after conversion will be stored.
   
2. For coustomizing the tool for other tagsets/languages , refer to the tool manual. 

Some points : 
1. The tool is copy and run.
2. Tool will still run if no arguments are given, default test files, wordlists and mapfile are provided with it.
3. Contact - {himanshu_s@students.iiit.ac.in} in case of problems in running , code errors or issues with conversions.

