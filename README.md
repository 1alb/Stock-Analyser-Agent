📈 Stock Analyzer Agent

A powerful Stock Analyzer Agent built using n8n that automates stock market analysis by collecting market data, calculating portfolio performance, analyzing market trends with Google Gemini AI, storing results in Google Sheets, generating charts, and sending daily reports via Gmail.

🚀 Features
📊 Tracks Portfolio Performance
💰 Calculates Profit & Loss
📈 Fetches NIFTY Market Data
📉 Fetches SENSEX Market Data
🤖 Generates AI-based Market Summary using Gemini
📑 Stores all market data in Google Sheets
📧 Sends Daily Stock Market Report via Gmail
📊 Generates Stock Market Charts Automatically
⏰ Runs Automatically on a Schedule
🛠️ Tools & Technologies Used
⚡ n8n
🤖 Google Gemini API
📊 Google Sheets
📧 Gmail
🌐 HTTP Request Node
💻 JavaScript Code Node
🔀 Merge Node
✏️ Edit Fields Node
🔄 IF Node
⏰ Schedule Trigger
📈 QuickChart API (for graph generation)
📂 Workflow Overview
Schedule Trigger
        │
        ▼
HTTP Request (Stock API)
        │
        ▼
Edit Fields
        │
        ▼
Store Stock Data (Google Sheets)
        │
        ▼
Calculate Profit/Loss
        │
        ▼
Store Portfolio
        │
        ▼
Fetch NIFTY Data
        │
        ▼
Store NIFTY
        │
        ▼
Fetch SENSEX Data
        │
        ▼
Store SENSEX
        │
        ▼
Merge Data
        │
        ▼
Gemini AI Summary
        │
        ▼
Generate Charts
        │
        ▼
Send Gmail Report
📋 Steps Followed
1️⃣ Create Workflow
Created a new workflow in n8n
Added a Schedule Trigger to execute automatically.
2️⃣ Fetch Stock Market Data
Added an HTTP Request node.
Connected it to a stock market API.
Retrieved stock information such as:
Stock Name
Buy Price
Current Price
Quantity
Sector
3️⃣ Edit Required Fields

Used an Edit Fields node to organize and rename data for easier processing.

4️⃣ Store Stock Data

Added a Google Sheets node to store stock market information.

Example Columns:

Stock	Sector	Buy Price	Current Price	Quantity
5️⃣ Calculate Profit & Loss

Used a JavaScript Code node.

Calculated:

Invested Amount
Current Value
Profit/Loss
Return %
Recommendation

Formula used:

(Current Price - Buy Price) × Quantity
6️⃣ Store Portfolio

Stored portfolio details in another Google Sheet.

Example:

Stock	Buy Price	Quantity	Current Price	Profit/Loss
7️⃣ Fetch NIFTY Data

Used another HTTP Request node.

Collected:

Index
Current Value
Change
Percentage Change
High
Low
Trend

Stored in Google Sheets.

8️⃣ Fetch SENSEX Data

Added another HTTP Request node.

Collected:

Index
Current Value
Change
Percentage Change
High
Low
Trend

Stored in Google Sheets.

9️⃣ Merge All Data

Used a Merge Node to combine:

Portfolio
Profit & Loss
NIFTY
SENSEX
🔟 Generate AI Summary

Added a Google Gemini (Message a Model) node.

Prompt included:

Portfolio Performance
Profit/Loss
NIFTY Analysis
SENSEX Analysis

Gemini generated:

📈 Market Trend
🏆 Top Gainers
📉 Top Losers
💡 Investment Suggestions
📄 100-word Daily Summary
1️⃣1️⃣ Generate Charts

Used QuickChart API via an HTTP Request node.

Generated charts for:

📊 Portfolio
📈 Profit & Loss
📉 NIFTY
📊 SENSEX
1️⃣2️⃣ Send Email Report

Added a Gmail node.

Email included:

🤖 AI Summary
📈 Portfolio Details
📊 NIFTY Report
📉 SENSEX Report
📎 Generated Charts
1️⃣3️⃣ Automate the Workflow

Connected all nodes.

Workflow now:

Executes automatically on schedule
Updates Google Sheets
Generates charts
Creates AI summary
Sends a complete daily email report
📊 Google Sheets Used
📁 Stock Market Data
💼 Portfolio
📈 NIFTY
📉 SENSEX
💰 Profit & Loss
🤖 AI Capabilities

Google Gemini analyzes:

📈 Overall Market Trend
📉 Index Performance
💰 Portfolio Growth
📊 Profit/Loss Analysis
💡 Investment Suggestions
📝 Daily Market Summary
📧 Output

At the end of each execution, the workflow automatically:

✅ Fetches latest stock market data
✅ Calculates portfolio performance
✅ Updates Google Sheets
✅ Generates market charts
✅ Creates an AI-powered market summary
✅ Sends a professional email report
📚 Skills Demonstrated
⚡ Workflow Automation
🌐 API Integration
📊 Data Processing
📈 Financial Analysis
🤖 Generative AI Integration
📑 Google Sheets Automation
📧 Email Automation
💻 JavaScript Scripting
🔀 Data Merging
📉 Data Visualization
🎯 Project Outcome

This Stock Analyzer Agent provides a fully automated stock market monitoring solution that collects live market data, tracks portfolio performance, performs AI-driven market analysis, stores structured records in Google Sheets, generates insightful charts, and delivers a comprehensive daily report directly via email—eliminating manual tracking and enabling faster, data-driven investment decisions.
