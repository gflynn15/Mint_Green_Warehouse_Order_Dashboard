# Mint_Green_Warehouse_Order_Dashboard
Operations Order Management Excel Dashboard

**Client Request**
Client wanted an excel dashboard that presented their order statuses into a simple and informative dashboard. Project's overall purpose is to decrease the clients time spent extracting the data from SAP and creating multiple pivot tables to analyze their order pool status. 

**Problem Statement:** 
Excessive indirect time for management is being spent extracting reporting and analyzing it. This time removes attention from the floor and leads to operational bottlenecks. 

**Solution Provided:**
Client stated that they wanted a solution that was excel based due to their comfortability with excel. Currently the client downloads a file from SAP daily. Then they summarize the data into mutiple pivot tables for review. I wanted to create them a tool that allows them to download the file to a designated directory. Once the file is placed in the directory they simply open the excel dashboard file and the data is read. After the data is processed, it is converted into a simple to read dashbaord that presents order pool status. 

**Steps Taken**
1. Create a power query connection that extracts the data from the downloaded file.
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
  - Sheet name is "KPI Board"
  - These graphs read through the order detail file and provides the below information for the operations manager to review:
  - <img width="933" height="609" alt="image" src="https://github.com/user-attachments/assets/324119ca-32b3-459a-93ae-5ae123ea67f0" />
  - **Header Bar:**
  - <img width="936" height="57" alt="image" src="https://github.com/user-attachments/assets/2396bc26-3447-438d-a446-b915919ea760" />
  	- Provides a quick snap shot into order metrics notifying the operations team how many late orders they need to shift their attention to fulfilling.
  	- Number of orders that need to be picked and packed.
  		- This assist the operations team with deciding where head count needs to be shifted to maintain operational flow.
  - **Trend Analysis:**
	- <img width="413" height="552" alt="image" src="https://github.com/user-attachments/assets/0cef6bb8-41d3-4658-8665-3ac9df12b341" />
  		- The left side of the table provides trend analysis into order, unit, and committed dollar amounts.
 		- Trend analysis assist the operations team with long term and short term labor planning.
    	- Order trends decide overall facility staffing needs.
    	- Quantity trends provide function specific analysis allowing the operation to effectively utilize facility staffing into key department groups.
    	- Dollar Amount committed is more useful for executive reporting to analyze movement of bif dollar value orders and what can be reported to shareholders.
- **Order Status by Process Step:**
  - <img width="517" height="555" alt="image" src="https://github.com/user-attachments/assets/09c9225c-f06a-443a-8e29-4cef696523fe" />
 	- Right side of the dashboard highlights the current progression of all orders in the opreation and where they are within the process.
   	- This view is curtial for the operations management team to utilize to ensure each department is staffed correctly to progress orders through the process to meet SLA.
   		- For Example:
   		- If the pack out process is showing a lack of work but the picking process step is show casing a lot of work to be done then this would provoke the operations managers to shift their pack out team into 			picking to build up work then shift them back into pack out once enough order volume has been built up to keep them utilized.
- Filters are available on all graphs for the operations management team to review the data in more detail by either date or function specific statuses.
- <img width="518" height="556" alt="image" src="https://github.com/user-attachments/assets/144e72ac-97e0-4fbf-844a-b5f3eb3ad99a" />
- <img width="937" height="642" alt="image" src="https://github.com/user-attachments/assets/307159b5-5bc6-426e-8cbd-54a6ad4c3484" />
- When any of these filters are changed, the graphs will refresh to reflect the change made by the filter. 


