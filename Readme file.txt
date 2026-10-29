Hi All
*********************Follow this steps******************* 

1-Go to https://trustfiles.github.io/pos-system
2-fill details and go to next page
3-Genarate My Pos prompt
4-Copy prompt
5-go to chatgpt and past and sent
6- you can see code.gs and index.html
7- make folder in your desktop and crate file index.html and past code your copy from chatgpt.
8-Search google sheet andSetup Instructions

Step 1: Create the Google Sheet
1. Open Google Sheets.
2. Create a new spreadsheet.
3. Name it POS Database.
You do not need to create any database tabs or column headers manually.

Step 2: Open Apps Script
1. Open your new spreadsheet.
2. Select Extensions → Apps Script.
3. Open the default Code.gs file.

Step 3: Add the backend
1. Delete the existing example code.
2. Copy the complete contents of the downloaded Code.gs.
3. Paste it into the Apps Script editor.
4. Click Save.

Step 4: Initialize the database
1. Select setupDatabase from the function selector.
2. Click Run.
3. Approve the requested Google permissions.
The script should create these sheets automatically:
- Settings
- Products
- Categories
- Sales
- SaleItems
- Customers
- Expenses
The Settings sheet will be seeded with the initial configuration.

Step 5: Deploy the backend
1. Click Deploy → New deployment.
2. Select the deployment type Web app.
3. Set Execute as to Me.
4. Set Who has access according to your security requirements. Anyone enables public access but is not recommended for an unprotected business database.
5. Click Deploy and complete any authorization prompts.

Step 6: Copy the Web App URL
Copy the deployed URL ending in /exec.

Use the deployed Web App URL, not the Apps Script editor URL.

Step 7: Configure the frontend
1. Open the downloaded index.html in a text editor.
2. Find the configuration near the beginning of its JavaScript.
const GOOGLE_SCRIPT_URL = "PASTE_YOUR_GOOGLE_APPS_SCRIPT_WEB_APP_URL_HERE";


3. Replace the placeholder with your actual /exec URL. For example:
const GOOGLE_SCRIPT_URL = "https://script.google.com/macros/s/YOUR_DEPLOYMENT_ID/exec";


Free Database perpose - google sheet
