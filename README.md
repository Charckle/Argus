#Argus - A Whoosh fulltext .txt files searcher for python 3.7

Argus is a module for searching trough a folder with .txt files with the Whoosh search engine, currently in its infant stage.

As far as it works now, you give it the folder, where the TXT files are stored (if you give him nothing, he will search in the folder "data"), and he returns the file name with the local path. If the folder's name is 
"data", it will return "data/a_txt_file.txt"

'''
import argus

banana = argus.WSearch()

banana.index_create()
rezultati = banana.index_search("banan*")

for zadetek in rezultati:
    print(f"Found in the file:{zadetek}")

'''

