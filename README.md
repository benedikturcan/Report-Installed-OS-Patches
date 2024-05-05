# Report-Installed-OS-Patches
This tool retrieves and generates reports on installed OS patches for organizations. It offers the flexibility to choose the output format as either CSV or PDF and to define a date range.

----------------------------------------------------------------------

**👉 Prerequisites:**<br>
Before using this code, ensure you have the following prerequisites installed:
</br>

Node.js: </br>
Ensure Node.js is installed on your system. You can download and install Node.js from the official Node.js website.

----------------------------------------------------------------------

**🚀 Usage:**

🔑 API Credentials: <br>
You need to provide your NinjaRMM API credentials, including the clientId and clientSecret. These credentials authenticate your access to the NinjaRMM API.

🌎 Region: <br>
Specify the region of your NinjaRMM account. This could be either "eu" for Europe or "app" for the US.

📅 Date Range: <br>
Choose the desired date range for the report. Options include:
- today
- yesterday
- currentWeek
- lastWeek
- currentMonth
- lastMonth

💾 Output Format: <br>
Decide whether you want the output in CSV or PDF format.

Instructions:
Install Dependencies:
After cloning or downloading the code, navigate to the project directory in your terminal.
Run npm install to install the required dependencies.
Configure Settings:
Open the index.js file in your preferred code editor.
Fill in the required API credentials, region, date range, and output format at the top of the code.
Execute the Script:
Run the script by executing node index.js in your terminal.
The tool will fetch data from the NinjaRMM API and generate reports based on your specified settings.
Outputs:
CSV Output: The tool generates a CSV file for each organization, containing details of installed OS patches.
Each CSV file is named after the respective organization.
The CSV file includes columns for organization name, patch status, installation timestamp, device ID, timestamp, and KB number.
PDF Output: If PDF output is chosen, the tool generates a PDF report for each organization.
Similar to CSV, each PDF file is named after the organization.
The PDF report presents the same information as the CSV but in a formatted table within the document.
Error Handling:
The tool handles errors gracefully, providing clear messages for any encountered issues.
For instance, if there's an invalid date range specified, it throws an error indicating the available options.
Dependencies:
node-fetch: Used to make HTTP requests to the NinjaRMM API.
fs: File system module for reading and writing files.
path: Module for handling file paths.
puppeteer: Headless Chrome Node.js API used to generate PDF reports.
Note:
Ensure your system has Node.js installed and configured correctly to run the script.
Make sure you have the necessary permissions and access rights to fetch data from the NinjaRMM API.
