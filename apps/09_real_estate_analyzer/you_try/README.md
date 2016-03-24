# App 9: Real Estate Analyzer App

![image](app-9-screenshot.png)
 
If you want to try this yourself, try to build the interactive app above. 

This application will load a CSV file of real estate data and then answer several questions by processing the data using list comprehensions and generator expressions.

* What is the **most** expensive house sold that year?
* What is the **least** expensive house sold that year?
* What are the features of an *average* house?
* What are the features of an *average **2-bedroom*** house?

Key concepts introduced
=================

**Dictionaries**

Dictionaries are data structures which allow random access by a key (string, number, whatever). They are extremely common and powerful in Python.

    info = dict()  # {}

**Lambdas**

Lambdas are small inline methods.

    def find_sig_nums(nums, predicate):

**CSV File Parsing**

    def load_file(filename):
        with open(filename, 'r', encoding='utf-8') as fin:
            reader = csv.DictReader(fin)
            purchases = []
            for row in reader: # row is a dictionary
                purchases.append(row)

        return purchases


**py2 vs py3**

    try:

    # Can use statistics.mean as needed
    
    numbers = [1, 6, 99, ..., 5]

**List comprehensions**

    paying_usernames = [
    # paying_usernames is a list

**Generator expressions**

    paying_usernames = (
