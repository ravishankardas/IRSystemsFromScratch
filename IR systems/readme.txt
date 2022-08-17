Dependencies:
All the dependencies required for the program to run are pandas, numpy, nltk, num2words. I have automated those installs but if any other library is missing install them by writing pip install library_name in the command line. i have used pandas to work with dataframes. numpy was used for some numerical calculation. nltk was used for tokenization, stemming and removing stopwords.

(for any query i am assuming there will be atleast one word which is present in the corpus otherwise my system will return no files)
(i am assuming the input file will be in a text file with the same format as queryid and query text separated by a tab)



preprocessing:
In the first question i have done preprocesing by performing tokenization, stemming, removal of stopwords. I have also removed all the special charcaters and single length digits and words from text. The preprocessing notebook takes a lot of time as it cleans the whole data. I have already cleaned the text and saved them in pickle files. there are four pickle files namely postinglist,fileindex,filenorms,filewordlist where posting list contains for every words contains in which documents and filewordlist contains all the words indexwise and fileindex contains for every document its file name and the number of words in it. Filenorms contains the norms for all the documents present in the corpora. If you want to run this file you should first put the extracted corpora folder in the same directory and then run it using jupyter.


How to run:

Put the input file in the directory then open the current directory in the terminal and type "make run ARGS=(input_file_name without the .txt extension)" this command will first install all the packages and then unzip the roll_name-ir-systems file and then run the scripts inside it and the make three csv files in the parent directory from where the makefile was called.
Run "make clean" in the terminal this will delete the all the csv files and zip the 21111052-ir-systems and then you can again run "make run ARGS=input_file".







