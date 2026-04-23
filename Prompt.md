I want you to create in one single HTML file a responsive web dashboard that reads data from a public Google Sheet and works well on both desktop and mobile. The final result will be hosted on Cloudflare Pages, so keep the solution simple and easy to deploy. I am not a programmer, so keep the architecture beginner-friendly and avoid overengineering



**Purpose:**
This dashboard is for tracking customer laptop returns. I add rows to this Google Sheet daily. 
The file currently has around 9,000+ rows and grows every day.



**Data source:**
The source is the Google Sheets file below.
Use only the worksheet/tab named "ReturnsRecord" as the data source.
Do not read from, merge with, or depend on any other sheet/tab in the spreadsheet.
Each row in "ReturnsRecord" represents one returned laptop.
The first row contains the column headers.

https://docs.google.com/spreadsheets/d/1bFiGJjn1bE1f7Ipmg1kY7r-e95_U0Ovk9ndZMOZGyRk/edit?gid=0#gid=0



**Columns:**

- A: Main Return Date (Physically arrived at our company)

- B: Order number on our system

- C: Marketplace name

- D: Order purchase date on the marketplace

- E: Order number on the marketplace

- F: Customer name and surname

- G: Date when the customer claim ticket was opened on the marketplace

- H: Order status on the marketplace

- I: Reason for return

- J: Total price of the customer order

- K: Physical status and location of the unit

- L: Link to the order on the marketplace

- M: Date when the record was added to this Google Sheet 

  

Important notes:
- Reasons for return in Column I are free text and may contain variations like “screen damaged”, “broken screen”, “crack”, etc.

- The app should handle at least 9,000 rows efficiently. 

- Optimize loading and filtering performance for large datasets in the browser

  

**What we need:**

1. Dashboard summary cards:
   - Total returns for today.
   
     Definition of "today":
     Each time the page loads, automatically use the current date in Europe/Warsaw timezone.
     Then compare that date with Column A (Main Return Date).
     Count all rows where Column A matches today’s date, and show the total in the summary card.
   
   - Count all rows where Column H exactly equals ‘W naprawie’
   
   - Count all rows where Column H exactly equals ‘W serwisie zewnętrznym’
   
2. Filters:
   - date from / date to (Column A)
   - customer name (Column F)
   - Order status on the marketplace (Column H)
   - Physical Status and location of the unit (Column K)
   
3. Search:
   - Keyword search inside Reason for Return (Column I), with support for partial match, case-insensitive search, and normalized text matching
   - Example: search “screen” and count how many related returns exist in the selected period.

4. Results table:
   - sortable
   - paginated
   - mobile-friendly
   - shows all fields clearly from A to M

5. Analytics:
   - Top repeated reasons for return (Column I) 
   - Top marketplaces by number of returns (Column C)
   - Returns trend over time based on Main Return Date (physically arrived at our company) in Column A

6. Design:
   - Very simple and fast
   
   - Suitable for managers checking quickly from a phone
   
   - Clean layout, not crowded
   
     

