# Information-retrieval-assignment

## Assignment 1: CRAWLER
Using a Python library (e.g. BeautifulSoup/Scrapy/...) to crawl data from a web page (e.g. vnexpress, tuoitre, kenh14...) and give some statistical information:
    
- Which classes/tags that indicate the place of content.
- Sort the classes/tags in the descending order of frequency in a website.
- Pick the most frequent class/tag in the list and write its contents into files.

## Assignment 2: BOOLEAN SPACE MODEL
Input:
   - List of documents as listed out from from the assignment 1 (e.g. title / summary / content of a newspaper).
   - Query in boolean format: 'MU' AND 'Liverpool'

Output: list of relevant documents based on input query.

## Assignment 3: VECTOR SPACE MODEL
Input:
   - List of documents in the assignment 1.
   - Query string (free style)

Ouput:
   - Relevant documents

## Assignment 4: EVALUATION
Content: Evaluation of an Information Retrieval System.

1. PREPARING

1.1. Go to https://archive.ics.uci.edu/ml/machine-learning-databases/20newsgroups-mld/ to download 20_newsgroups.tar.gz file and extract it.

1.2. Merge all articles into one collection.

2. INDEXING

2.1. Perform building index for the text collection using learned techniques.

3. EVALUATION

3.1. Build a set of queries of your own with the following conditions:
-	Each query belongs to only one class of the original dataset
-	There is not any class belonging to no query.

3.2. Perform retrieval using that set of query, output the performance by:
-	Render the graph of Precision/Recall curve.
-	Print out other measures: F-measure, MAP

The Relevance of each retrieved document is determined by this rule:
-	1 if that document contains at least one words of the query AND that document belongs to the same class/category as the query
-	0 otherwise
