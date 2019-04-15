# language-classify

Based on the FANN tutorial (http://fann.sourceforge.net/fann_en.pdf). 

The goal is to create a NN that given a text file of English, French, or Spanish will be able to determine which of those 3 languages it is. It does so based on the frequencies of the 26 letters of the alphabet. 

The program in frequencies.pi goes through as many sample files as desired and generates the frequencies of the letters. (For each sample file you want the program to run through, you have to specify its name, e.g. english1.txt, and which language it actually is, by entering either "e", "f", or "s". I've provided 9 sample files, 3 of each language; I got the text from random Wikipedia articles in each language.) This program generates a text file called frequencies.data. 

Then, lang_classify_train.pi can be compiled and main can be run to create a NN. 

The program in lang_classify_test.pi can then be compiled and used; it asks for the name of a text file, finds the frequencies, and runs that information through the NN to classify the language as either English, French, or Spanish.
