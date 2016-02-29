An iPython Notebook for tracking health related things.
Must have MongoDB and PyMongo installed and running for this notebook to work properly.

Some foods have been added to the top for ease of use, however this is a very inexhaustive list.
In the future, foods will most likely get their own database.
For now however, feel free to modify the list of foods as you like.


Instructions:

*)  If you don't have MongoDB, use your OS's native package installer to download it
    i.e. "apt-get install MongoDB" or "yum install MongoDB" or "brew install MongoDB"
**) If you don't have PyMongo, download it with python's pip installer:
    "python -m pip install pymongo"

1)  Start MongoDB with 'sudo mongod'
2)  Start up your notebook and navigate to this directory
3)  Run the 'Initial setup' cell.
4)  Run the 'Utility Calculations' cell to get an initial estimate for your macros (algorithm borrowed from IIFYM.com and Wikipedia)
5)  Add your weight for today to the top of the 'Tracking' cell.
6)  As you go through your day, record your meals by adding them to the meal variables in the Tracking cell.
7)  Optionally, include sleep and bodyfat percentage in the top portion of the Tracking cell.
8)  Use the 'Database Insertion' cell to insert your day's data into MongoDB. This should "just work" if you you have MongoDB     running on another terminal window and PyMongo installed.
9)  Use the 'Data Retrieval' cell to retrieve your data.
10) Optionally, graph your data with the graphing cell! This will show you your stats over time. You can change what is shown     by editing the "ax.plot" lines and corresponding "ax.set_title" lines.
11) That's it! Be sure to look for trends in the graphs. They'll be invaluable in helping to reveal what is causing what.
