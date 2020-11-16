# Investment Data Visualization for Trading212 with Microsoft Power BI

The first thing to be done, is to create a table with the necessary data to be analyzed. This data comes from the extracts sent via email by Trading212 the day after you buy or sell a stock.

Each time a new extract is issued, it needs to be added to an input Google Sheet table. In this case I decided to use Google Sheets to keep everything in a cloud, and also because it includes the function GOOGLEFINANCE() that allows to make some calculations needed to get stock values live. The template of this table can be copied to your own Google Drive from here.

The next step is to copy the information from the above table into your own Google Sheet document. The best way to do it is:

1.- Copy the table content into your desktop Excel

2.- Delete the empty rows

3.- Replace the currency by its symbol (in this case, "€" instead of "EUR")

4.- Remove the last column 'Total cost'

5.- Optional: in case your language is not English, make sure that the number format is correct


The data should perfectly fit the Google Sheets tab "Trading212", only occupying the gray headers. Then, it is necessary to manually fill up each of the blue header columns, using the dropdown menus. Finally, the green header columns should be automatically filled by the calculations.

Then, the tabs "Dividends" and "Deposits" should be filled up accordingly. The last tab, "Symbols", contains over 1,700 different stocks, ETFs, ETCs and Bonds. In case there is something missing, it just needs to be added at the end of the table.

The next step is to connect your own Google Sheet table to Microsoft Power BI, meaning that your table has to be published. For this, all that needs to be done is to click on "File", "Publish in the Web" and click "Publish" leaving everything in default. This will generate a link to your table that will be needed later. This makes the table visible for anybody that has the URL generated, so make sure not to published anywhere.

If you don't have Microsoft Power BI downloaded at this point, it is a good time to do it. After the installation is completed, open this PBIX file and connect it to your published table. To do that, follow this steps:

1.- Select the "Data" tab

2.- Click on "Get data" and select "Web":

3.- Introduce your published Google Sheets links and select the tables "Transactions", "Dividends" and "Deposits"

4.- Go to "Transform Data", and for each of the three tables, copy the query corresponding to each one (Transactions, Dividends and Deposits) in the "Advanced Query" option 

5.- Click in "Close and Save"


At this point, you should be able to see all your data in the three tables, and you can start exploring your dashboards.

I hope this tool becomes really helpful. I will continue to work on it and improve it. And any help and comments are more than welcomed.
