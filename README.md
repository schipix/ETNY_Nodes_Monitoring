# This webpage monitors the status of a list of Ethernity Cloud Nodes.

# It is a tool I created originally for my own use, which then I decided to share with the community.
# DISCLAIMER: I am not part of the Ethernity Cloud Team. I only act pro-bono in the interest of the Ethernity community.
# Technically speaking the webpage launches API calls to the Bloxberg Chain, fetches the last timestamp of a transaction call for a given node/list of nodes and eventually builds a three-column HTML table that contains the hostname of the node, the Ethernity Cloud Node address and when was the last transaction call executed.
# Prerequisites: the webpage is stand-alone and doesn't need to be uploaded on a webserver to work, if opened on a desktop (regardless what OS).On Android it should work as well just by opening the html file in a browser. EXCEPT...
# Except when the security settings turn agains you :) In this case you just have to install a lite web server. I personally use SimpleHttpServer which is easy to use and very straigh forward.
#  On iOS it hasn't been tested yet.


# HOW TO modify the webpage so it shows your own nodes:
#   - Open the html file in an text editor (e.g. Notepad)
#   - Search for "const nodes_array"
#   - For each node you want to monitor add a new line using the three templates as a model
#   - Delete the three lines representing the templates.


# Future developements as of 12.07.2023:
#   - Load the nodes list from an external JSON file

# Future developements as of 02.08.2023
#   - Adapt the queries to accommodate the API query limit of 20 calls
