Rental Price Analysis

Data Source:
Quarterly Rental Price: https://discover.data.vic.gov.au/dataset/rental-report-quarterly-quarterly-median-rents-by-lga
2016 Census Quick Stats: https://quickstats.censusdata.abs.gov.au/census_services/getproduct/census/2016/quickstat/036

Analyze official Local Government Area of North and West Metro of Victoria

- Extract, Transformation, Load -
        Querying Quarterly rental price by separating each stated attributes. Cross multiplying all and removing "Group Total and Total". Load it to workbook and power BI.
        Created Relationship between suburb from rental price table and census table.
- Visualization -
        First Page
        Map : Suburb as axis, Limit Arcgis Search to one country and boundary format , Average Rent across all period from 2017
        Line Graph: Period as Axis, Suburb as Legend, Median Rent Price as Value Summarize by Average, Filter Type = median
        Forecast Chart: Forecast Period as Axis, Suburb as Legend, Simple Linear Regression Measure as Value summarize by Average
        Growth Rate: Slope of simple linear regression is returned instead
        Standard Deviation: Median Price Summarized by standard Deviation

        Second Page
        Period Filter from 1/1/2016 - 31/12/2016
        First Line Graph (Top Left): Suburb as Axis, Rental Price as value summarized by Average,  Median Age as secondary Value
        Second Line Graph (Middle Left): Suburb as Axis, Rental Price as value summarized by Average,  Median Mortgage Price as secondary Value
        Third Line Graph (Bottom Left): Suburb as Axis, Rental Price as value summarized by Average,  Median Household Income as secondary Value
        Pie chart (Top Left): Suburb as Legend , Sum of Population as value
        Pie chart (Top Left): Suburb as Legend , Sum of All Private Dwellings as value
        Bar Graph (Bottom Right): Suburb as Axis , Median Rent Price as Values summarized by Average, Filter by Type = Median

        Third Page
        Chart Picture from http://publictransportresearchgroup.info/benchmarking/melbourne/public-transport-service-level-trends-in-local-government-areas-in-melbourne/

        Last Page:
        Map : Suburb as axis, Limit Arcgis Search to one country and boundary format , Average Rent across all period from 2017
        First Data (Top to bottom): Average of Median Rent
        Second Data: Median of Mortgage Payment
        Third Data: Median of Age, Goal is average of age of all Suburb
        Fourth Data: Sum of Population
        Fifth Data: Standard Deviation of Median Rent price
        Sixth Data: Slope of simple linear regression is returned instead

- Analysis -
        Analyze data per suburb and trend of data per suburb over a period of time from 2017 to 2019. Indicating a Linear trend for all areas. Therefore chosen Linear regression as a method of forecasting.
        Map is chosen due to the nature of the task and to show factor of location. Areas closer to a sea or port tend to have higher rent.
        Linear graph used to detect trends between two factors to indicate correlation between each factors and rental analysis. Conclusion is that Age and Mortgage payments show a clear trend to rental price variation by suburb.
        Pie chart used to indicate proportion of population and sum of private dwellings.
        Bar graph used to indicate which areas has the highest average rent in 2016.
        Transport service picture is chosen instead due to the data being hard to find or unavailable. Conclusion is that it does not show any pattern of correlation between rental price and number of transportation services in the area.
        Final data is chosen to help company use this analysis for specific decision making that involves financial needs.

File:
        AI Australia BI task.pbix : Microsoft Power BI file used.
        Quarterly Median Rents by local government area: Excel file that power BI pull from.
        AI Australia response video: Video required for response.
