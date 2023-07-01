Instructions

To clone the git repo to your local machine, follow the steps here: https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository


Make sure you have a chromedriver.exe that supports your Chrome browser: https://chromedriver.chromium.org/downloads
1. Open the glassdoor_login.json file and input your login information.
2. Create a Google Service Account by following the steps found here:
  - https://cloud.google.com/iam/docs/service-accounts-create#:~:text=In%20the%20Google%20Cloud%20console%2C%20go%20to%20the%20Create%20service%20account%20page
  - This will require you to create a "NEW PROJECT"
  - Then, once the account is created, you click on the "email" and click on the "KEYS" tab
  - Click on "ADD KEY", create a new key
  - After selection JSON, a json file will download
  - rename that file to "credentials.json" and move it into this current directory
  - Create a new spreadsheet and share edit access to the client_email found in the json file or found on the service account UI
3. Open the web scrape jupyter notebook and replace SPREADSHEET_NAME and SHEET_NAME with your spreadsheet's name and sheet name for where you want the data to write
4. Update the following variables with your values: JOB_TITLES, LOCATIONS, GOOD_KEYWORDS, TITLE_BAD_KEYWORDS, COMPANY_BAD_KEYWORDS, BAD_KEYWORDS
5. Run the notebook
