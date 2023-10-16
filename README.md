# Data_Science_bootcamp

### Project 1 - Web Scraping with Python
In this project, you will apply your knowledge of Python and its ecosystem of libraries to scrape information from a website and create a dataset of CSV file(s). Here are the steps you'll follow:

- Pick a website and describe your objective

Browse through different sites and pick on to scrape. Check the "Project Ideas" section for inspiration.
Identify the information you'd like to scrape from the site. Decide the format of the output CSV file.
Summarize your project idea in a paragraph using a Markdown cell and outline your strategy.

- Use the requests library to download web pages

Inspect the website's HTML source and identify the right URLs to download.
Download and save web pages locally using the requests library.
Create a function to automate downloading for different topics/search queries.

- Use Beautiful Soup to parse and extract information

Parse and explore the structure of downloaded web pages using Beautiful soup.
Use the right properties and methods to extract the required information.
Create functions to extract from the page into lists and dictionaries.
(Optional) Use a REST API to acquire additional information if required.

- Create CSV file(s) with the extracted information

Create functions for the end-to-end process of downloading, parsing, and saving CSVs.
Execute the function with different inputs to create a dataset of CSV files.
Attach the CSV files with your notebook using jovian.commit.

- Document and share your work

Add proper headings and documentation in your Jupyter notebook.
Publish your Jupyter notebook to Jovian and make a submission.
(Optional) Write a blog post about your project and share it online.

### web scraping with selenium and aws

Please refer to the below link for the updated code.

Code: https://github.com/aakashns/selenium-youtube-scraper-live

Web scraping is a great way to extract public information from websites and create datasets for data analysis and machine learning. In this live hands-on workshop, we walk through the process of building and deploying a web scraping project from scratch using Python, Selenium, and AWS Lambda.

- Objective
Scrape top 10 trending videos on YouTube using Selenium
Set up a recurring job on AWS Lambda to scrape every 30 minutes
Send the results as a CSV attachment over email (or to a spreadsheet)
- Prerequisites
Python

- Topics Covered
GitHub
Replit
Selenium
AWS Lambda
SMTP
- Step 1 - Create a GitHub repository
Create a repository at https://github.com/new
Add README, gitignore (Python) and license
(Optional) Clone the repository locally
References:
Introduction to GitHub: https://lab.github.com/githubtraining/introduction-to-github
Git & GitHub tutorial: https://www.youtube.com/watch?v=RGOj5yH7evk
- Step 2 - Launch the repository on Replit
Note: Chromedriver & chromium doesn't come pre-installed with Replit after a new update. Please follow these steps to add chromedriver & chromium to replit: https://jovian.ai/birajde9/replit-add-chromdriver-chromium

Connect Replit with your GitHub account
Launch the repository as a Replit project
Set up the language and run command
Create and execute a Python script
Attempt to scrape the page using requests & Beautiful Soup
Sometimes the code will not scrape all the videos if the page is not loaded completely. Import the time module & use the time.sleep(5) command to load the page completely and then find the elements.
References:
Introduction to Replit: https://docs.replit.com/tutorials/01-introduction-to-the-repl-it-ide
Replit + GitHub: https://docs.replit.com/tutorials/06-github-and-run-button
YouTube trending feed: https://www.youtube.com/feed/trending
Beautiful soup tutorial: https://blog.jovian.ai/web-scraping-using-python-and-beautifulsoup-adf43cbdb816
- Step 3 - Extract information using Selenium
Install selenium and create a browser driver
Load the page and extract information
Create a CSV of results using Pandas
References:
Selenium tutorial: https://www.browserstack.com/guide/python-selenium-to-run-web-automation-test
Pandas tutorial: https://jovian.ai/learn/data-analysis-with-python-zero-to-pandas/lesson/lesson-4-analyzing-tabular-data-with-pandas
- Step 4 - Send results over email using SMTP
NOTE: Google security policy has been updated and the discussed procedure won't let you send emails using just a username and password now. Follow this blog for the steps to send results over email using SMTP: https://blog.jovian.ai/web-scraping-using-selenium-2a3ffa1f03f4

Create email client using smtplib
Set up SSL, TLS and authenticate with password
Send a sample email with just text
Send an email with text and attachment
References:
Sending Email with Python: https://stackabuse.com/how-to-send-emails-with-gmail-using-python/
Send email using Python: https://www.geeksforgeeks.org/send-mail-attachment-gmail-account-using-python/
Environment variables on Replit: https://docs.replit.com/programming-ide/storing-sensitive-information-environment-variables
https://docs.aws.amazon.com/lambda/latest/dg/configuration-envvars.html
Update Google sheets using Python: https://www.analyticsvidhya.com/blog/2020/07/read-and-update-google-spreadsheets-with-python/
- Step 5 - Set up a recurring job on AWS Lambda
Create an AWS Lambda Python function
Deploy a sample script and observe the output
Add layers for Selenium and Chromium
Set up recurring job using AWS CloudWatch
References:
Python on AWS Lambda tutorial: https://stackify.com/aws-lambda-with-python-a-complete-getting-started-guide
Chromium & Selenium on AWS Lambda: https://dev.to/awscommunity-asean/creating-an-api-that-runs-selenium-via-aws-lambda-3ck3
Recurring AWS Lambda functions: https://docs.aws.amazon.com/lambda/latest/dg/services-cloudwatchevents-expressions.html
Selenium Lambda Layers: https://github.com/aakashns/selenium-aws-lambda-layers

The workshop lasts approximately 3 hours and all code will be written live during the workshop. You will be able to follow along with the recording to work on your own web scraping project.
