# Invoice-Autopilot-workflow
n8n automation that reads invoices for you, so nobody has to type the data in by hand.

<img width="805" height="223" alt="Screenshot 2026-10-03 at 2 00 11 PM" src="https://github.com/user-attachments/assets/08e5df6f-9fee-4cdb-a18f-9fb8b8cce896" />

The workflow steps:  
1- An email with a PDF invoice arrives in your demo inbox.  
2- The workflow pulls the text out of the PDF.  
3- An AI model reads the text and returns clean fields: vendor, date, items, tax, total.  
4- A code step checks the math, such as whether the items add up to the total.  
5- If everything checks out, the invoice is saved to the Data Table.  
6- If something looks wrong, a Slack message goes to a person to approve or fix it.  
