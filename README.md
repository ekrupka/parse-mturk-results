Mturk Results Parser
================================

When running the getResults command via the Amazon Mechanical Turk command line interface, the results are returned in an unclean format. 

If you run the getResults command with the namevaluepairs option

	-namevaluepairs

Then this program will be able to parse the data, save it to a json file so that you have a clean data format to run other commands for your Mturk questionnaire (such as calculating bonuses to give), and it can save the answers to a csv file.

The parse method requires the output file that is recieved from running the getResults command with the options above. It also requires the name of the json file.

The save_to_csv function requires an answer list of the getresults keys (workerid, assignmentid, the name of your mturk questions, etc - these keys can be seen in the json file, since the json file saves all the results that comes from the output file of the getresults command ) that you would like to be saved to the csv file. 
