# GoodLight Challenge

This challenge involves two parts of roughly equal length. The first is a coding exercise, followed by a data analysis and modelling exercise. The challenge is not timed, but you are not expected to spend more than 6 hours in total.

Your submission should be in the form of a zipped folder containing your code, instructions on how to run your code, a requirements file, and any other documentation you consider relevant. A standalone git repository with descriptive commit messages is encouraged.

**Note:** Your code should be compatible with Python 3.6 or later.

## Part 1

The first part of your challenge involves building a scraper written in Python that will fetch living person records from [True People Search](https://www.truepeoplesearch.com/) ([example person URL](https://www.truepeoplesearch.com/results?name=Jerry%20Perullo&rid=0x0)). You should create at least one public class called `PeopleFinder` with at least one public method called `query`. This method should take in a first, middle, and last names, a date of birth, and a city and a state where a person lives, and should return a data dictionary containing the following information on a person:

* current and past addresses, including start and end date
* phone numbers
* email addresses
* associated names
* relatives
* associates
* businesses

### Notes:

* True People Search employs some anti-scraping measures. If you are unable to work around them to reliably gather data, you may query [Family Tree Now](https://www.familytreenow.com/) instead ([example person URL](https://www.familytreenow.com/search/people/results?first=Jerry&last=Perullo&rid=0s0)). In that case, email addresses and businesses will not be returned from the data source.
* You may use third-party libraries.
* If no correct match is found, you should return a `None` object.
* If there is more than one person matched for a query, you may return the first match.
* Your code should be well documented and understandable.

## Part 2

The second part of the challenge is more open-ended. You are expected to perform some analysis on data collected for at least a few hundred individuals using the data collector you built in Part 1. For example, this may be in the form of building a regression model to predict some target variable of your choice, building an unsupervised model to cluster data, or finding some other pattern in the raw data. You may also use other data sources to enrich your data (e.g. Zillow, Census data, etc.).

### Notes:

* If you are unable to build a dataset of individuals using the code you wrote in part 1, please submit your code for part 1 and we will provide you with a dataset for part 2.
* You may collect data on random individuals or on specific individuals within some group (for example, from a specific city, age group, or some other factor they might have in common).
* The goal of this task is to be able to extract any insights and patterns from the raw data that you find interesting.
* You should to able to back up any conclusions using data-based arguments and highlight any criticisms or flaws in your analysis.
* Finally, talk about any other things you would have looked at if you had one more week to work on this task.
