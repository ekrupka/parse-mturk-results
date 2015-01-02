Mturk Results Parser
================================

When running the getResults command via the Amazon Mechanical Turk command line interface using the `namevaluepairs` option, the results are returned in an unclean format. This program allows you to parse the results to json and csv file. The program is specifically tailored to print results for an [mturk experiment](https://github.com/ekrupka/mturk-survey-experiment/).

# Functions
In order to run the program all you need to do is `import parse`.

## parse.parse(output_file)
Requires the name of an outputfile to write the json results to a file names `output.json`.

## parse.save_to_save(json_file, [results=[]])
Requires a json_file and to read and writes the json file to csv file names `results.csv`. 

You can optionally pass in a list of results specifying the keys in the json results that should be written as 


The save_to_csv function requires an answer list of the getresults keys (workerid, assignmentid, the name of your mturk questions, etc - these keys can be seen in the json file, since the json file saves all the results that comes from the output file of the getresults command ) that you would like to be saved to the csv file. 
