# Social-Unrest-Event-Extraction-and-Summarization
The Armed Conflict Location &amp; Event Data Project (ACLED) is the highest quality, most widely used, real-time data and analysis source on political violence and protest in the developing world. Practitioners, researchers, and governments depend on ACLED for the latest reliable information on current conflict and disorder patterns [1]. However, the task of populating the database with events is currently carried manually by human volunteers across the globe. This makes the whole process time consuming and requires human efforts to train the volunteers and curate the data collected from them. Hence, we present a system which will automate the complete task of collecting data related to unrest events from various online sources and providing summarized text for every event. Additionally, every event will also be identified whether it is related to election violence or not. Experimental results on past data from ACLED demonstrate the effectiveness of our system.

Steps to follow before running the code-
Paths to be set in the code before running the main function –
-->Set your Google geocoding API key
      In class GetLongAndLat.java, set your google geocoding API key at 2 places (Search for “Your-API-KEY”).
-->Set the path of Chrome driver for Selenium in two files-
      TOIExtraction.java 
      ExtractDataFromAcled.java
      Search for “Set-Your-Chrome-Driver-Path-Here” in both the files
-->Set CSV File paths
      ParameterEvaluation.java
      OutputDataToCSV.java
      ExtractDataFromAcled.java
      Search for “Set-CSV-FilePath-Here” in the above 3 files.
-->Install the following python libraries before you run the code-
      Numpy
      Sklearn
      Pickle
      Pandas
      Nltk
      Networkx
      Practnlptools

Run the application-

--->Import Aparecium folder project as a maven project in any Java IDE.
--->Set the date for which you want to extract events for in TOIdataExtraction.java file.
    Search for comment – “//Set the date here”
---->Run the MainFunction.java’s main function in order to run the whole application.
---->A CSV file with name “ApareciumArticles.csv” will be generated on the path you mentioned for CSV files in the code in step 3. This file contains only the article content and article’s published date of all the articles collected by the application in it.
---->Also, in the end, another CSV file called “Aparecium.csv” will be generated on the same path as step 3 which will contain the events and respective event parameters along with summarized text in it for every event. The headers for this file are as follows –
      Article Content
      Published Date
      Actor
      Event Date
      Location
      Longitude
      Latitude
      Election Violence
      Summarized text
