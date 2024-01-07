# Project step
* Measure length of documents[*]
* Compute target lengths[*]
* Repeat the shrinking for input document until the summary size is within the context window[*]
   * Check the size of the collected summery 
   * slice document according to the limit size
   * sumerize the slices
* Repeat the shrinking for style document until the summary size is within the context window[*]
* Repeat the shrinking for final text base on input text and style text and thier target length[*]
* implimenting summerization process[*]

# Documentation
this code has 2 part 

* First part of this project is summerizing text with extractive summerization approach that extractive_symmerization.py is responsible for. The process includes:
    * calculate frequency of words in the text
    * tokenize  the sentences
    * calculate the score for each tokenized sentence base on the words frecuncy 
    * calculate the score for each tokenized sentence base on the words frecuncy 
    * select 10 most scored sentence 

* Second part is responsible for the process of handling the length of two document and shrinking them until proper size, the main.py in the responsible for that. Including these steps:
    * Measure length of documents
    * Compute target lengths
    * Repeat the shrinking for input document until the summary size is within the context window
    * Repeat the shrinking for style document until the summary size is within the context window[*]
    * Repeat the shrinking for final text base on input text and style text and thier target length[*]



# Running Project
In windows run these commands in rout of project:
* pip install -r requirements.txt
* py ./main.py

In Linux base systems:
* pip3 install -r requirements.txt
* python3  ./main.py
