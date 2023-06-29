# python--web_crawler_youtubelinks
#problem statement:
         ● Create a web crawler using python that is able to scrape first 10,000 results for the followinggoogle search input - site:youtube.com openinapp.co
        ● Collect all the given YouTube links of the above search link.
        ● Give the results in the JSON/CSV format.  

#workflow:
import requests
from bs4 import BeautifulSoup
import json

# Define the google_search function

# Set the search query and number of results

# Perform the Google search

# Create the output JSON 

# Save the results in a JSON file and csv file 

# Display a success message

Certainly! Here's a workflow for the web crawler that scrapes YouTube channel links from Google search results and saves them in JSON format:

Define the search query: Determine the search query that you want to use. For example, "site:youtube.com openinapp.co" to search for YouTube channels related to the website "openinapp.co".

Set the number of results: Determine the number of search results you want to retrieve. For example, 10,000.

Perform the Google search: Use the google_search function to scrape the search results for the given query and number of results. The function will return a list of dictionaries, where each dictionary represents a YouTube channel with the keys "Channel Name" and "URL".

Create the output JSON: Create a dictionary to store the output JSON. Assign the list of YouTube channel dictionaries to a key in the output dictionary. For example, {'YouTube channel links': search_results}.

Save the results in a JSON file: Open a file in write mode and use the json.dump() function to write the output dictionary into the file in JSON format. Specify the desired file name, for example, 'youtube_channel_links.json'.

Display a success message: Print a message to indicate that the results have been successfully saved in the JSON file.

Here's the overall code structure to follow:
