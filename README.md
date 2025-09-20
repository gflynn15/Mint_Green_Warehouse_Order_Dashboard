# Mint_Green_Warehouse_Order_Dashboard
Dashboard developed to assist the operations team with quickly analyzing their order status pools. 
**Client Request**
Cleint wanted an excel dashboard that presented their order statuses into a simple and informative dashboard. Project's overall purpose is to decrease the clients time spent extracting the data from SAP and creating multiple pivot tables to analyze their order pool status. 

**Problem Statement:** 
Excessive indirect time for management is being spent extracting reporting and analyzing it. This time remove attention from the floor and leads to ineffective business practices.

**Solution Provided:**
Client stated that they wanted a solution that was excel based due to their comfortability with excel. Currently the client downloads a file from SAP daily. Then they summarize the data into mutiple pivot tables for review. I wanted to create them a tool that allows them to download the file to a designated directory. Once the file is placed in the directory they simply open the excel dashboard file and the data is read. After the data is processed it is converted into a simple to read dashbaord that presents order pool status. 

**Steps Taken**
1. Create a power query connectiong that extracts the data from the downloaded file.
   <img width="491" height="452" alt="image" src="https://github.com/user-attachments/assets/7f1aef0f-53f5-4878-a33d-3fd36dc98086" />
2. Select the file containing the raw data
   <img width="935" height="586" alt="image" src="https://github.com/user-attachments/assets/09529c07-bb09-4d7f-9fc8-d48cf97227fc" />
3. Cleaned up the data through power query.
   - The order status descriptions columns contained a lot of whitespace errors that did not allow the graphs to calculate status correctly.
     This required me to use the replace function to get rid of all the white space.
   - <img width="1225" height="593" alt="image" src="https://github.com/user-attachments/assets/651e1be1-dd51-4d84-b4dd-3f6124e351fd" />
4. Pivot tables are then created to aggregate the status of each order by release date.
   - This is utilized to identify late orders and see what step they are within the process.
     	- Ensures focus is placed on these orders and labor is allocated appropriately.
  - <img width="794" height="616" alt="image" src="https://github.com/user-attachments/assets/f5902378-53cb-4a76-8daa-bc9a171f21ed" />
5. New Dashboard sheet is created
	- Graphs are created from each of the pivot tables in the previously created sheet.
  - 
