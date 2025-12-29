# Music Genres and Mental Health

## Research Question
How do different music genres affect mental health and emotional wellbeing?

## Approach
- Data cleaning and preprocessing
- Exploratory data analysis (EDA)
- Visualisation of genre vs mental health metrics
- Interpretation of observed trends

## Tools
- Power Query
- Power BI
- Excel
  
## Executive Summary
This project explores whether there is a correlation between music and the effects it has on mental health. Exploring how different genres, BPM and other factors affect the outcome. This is based on a self-impact assessment of over 700 people. Using further research to add to the analysis for a deeper insight. This data can be used to further help the understanding of music and the positive or negative outcomes it has in the current climate. 
There will be use of different modelling techniques to try gain deeper understanding of what the data depicts through web scraping and regression. These method will help determine if specific musical attributes are associated with a positive or negative effect on mental health and why these patterns emerge. Insights from the results could inform and develop mental health strategies in the industry. Ethical considerations including, data privacy are integrated throughout to ensure the use of sensitive information. 

## Data Infrastructure and Tools
For this particular dataset the main dataset was sourced from Kaggle. Music & Mental Health Survey (Rasagaitis, 2022). This covered data such as time of listening, age, favoured genre, alternative genres and the effects and rating of the person’s mental health. This is a structured dataset exported as a CSV file and is a structured format but still requires transformations before analysis for consistency and usability. Spotify is the largest streaming service in the world (Soundcamps, 2025). It discusses in more detail the demographic of listeners, top genres and artists and will be accessed via API’s enabling cross referencing alongside the original dataset. 
Power Query is a data transformation and preparation engine, allowing you to perform ETL (Extract, Transform and Load) processing. Also it is a repeatable process and can easily be refreshed in the future to get up-to-date data. (Microsoft Learn, 2025) This tool was selected for the transformations because it provides intuitive, repeatable processes for data preparations, handling null values, correction of formatting. It refresh capabilities support future updates with no to little manual intervention, aligning with best practices for reproducing the report. Given the dataset is relatively small Power Query works as the most effective tool in comparison to SQL which is better suited for larger scale and multi-source integrations.
Power BI was chosen for visualisation for its ability to create interactive dashboards with clear visual narratives. The end user will find it intuitive and interactive allowing them to explore insights dynamically and make informed decisions or easily capture outputs for documentation. Both of these tools providing a robust infrastructure for transformation and communication. Throughout adhering to the ethical considerations such as any anonymization and secure data handling. This data is stored in a cloud server ensuring safe access and reliable availability for further analysis.  

## Data Engineering
So this dataset was ready for analysis, several processing steps were under taken to maintain accuracy, completeness and consistency which are essential for high quality data.
The first transformation step was the create a new date column. The original was in a U.S format (MM/DD/YYYY), so required the standardisation to the more widely recognised DD/MM/YYYY for consistency and chronologically correct analysis. (Image 1)  
This was achieved by creating a custom column that extracted and reformatted part of the existing time stamp, finding the text between the “/” and reconstructs it to format the U.K standard format. (Image 2) It also needed to be converted from a text data type into a date. This was critical as leaving it would cause issues in the down streaming process such as filtering of day, month and year, grouping and time series visuals. 
Next data validation was applied across all columns for viable outputs. For example the mental health ratings were checked to make sure they fell within the range of 0-10 and were whole values. (Image 3) Null values were addressed with caution. While some blanks were acceptable, like optional demographic fields, essential columns like Music Effects required complete data as they formed the basis of analysis. (Image 4)
By applying structured ETL process the project adhered to best practices for reproduce ability, scalability and minimising risk. The workflow can be refreshed easily, manual intervention has been reduced all supporting future updates. This all aligns with modern trends in engineering such as automation and cloud integration and these transformation steps also minimise and enhance downstream analysis. Cloud computing has revolutionised data engineering and the infrastructure offers scalable and cost effective platforms for data storage and processing so data engineers can easily scale up or down based on changing volumes (Binariks, 2025)

## Data Visualisation and Dashboards

## Data Analysis

## References

## Appendix

## Status
- Work in Progress
