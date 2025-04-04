# BI-Project-GoogleFiber
End-of-course project for Google Business Intelligence Professional Certificate


# Part 1

## Welcome to Google Fiber! 

You are interviewing for a job with Google Fiber, which provides people and businesses with fiber optic internet. As part of the interview process, the Fiber customer service team has asked you to design a dashboard using fictional data. The position you are interviewing for is in the customer call center, where Fiber uses business intelligence to monitor and improve customer satisfaction.
To provide the interviewers with both BI value and organizational data maturity, you will use your knowledge of the BI stages: capture, analyze, and monitor. By the time you are done, you will have an end-of-course project that demonstrates your knowledge and skills to potential employers.

## Your meeting notes
You are interviewing with the Google Fiber customer service team for a position as a BI analyst. At the end of the first interview, you spoke with the BI team and hiring manager to gather details about this project. Following are your notes from the meeting. Use the information they contain to complete the Stakeholder Requirements Document, Project Requirements Document, and Planning Document.

## Project background:
The team needs to understand how often customers phone customer support again after their first inquiry; this will help leaders understand whether the team is able to answer customer questions the first time. Further, leaders want to explore trends in repeat calls to identify why customers are having to call more than once, as well as how to improve the overall customer experience. I will create a dashboard to reveal insights about repeat callers. 

This fictional dataset is a version of actual data the team works with. Because of this, the data is already anonymized and approved. It includes:
* Number of calls
* Number of repeat calls after first contact
* Call type
* Market city
* Date

## Stakeholders: 
* Emma Santiago, Hiring Manager
* Keith Portone, Project Manager
* Minna Rah, Lead BI Analyst

## Team members: 
* Ian Ortega, BI Analyst
* Sylvie Essa, BI Analyst\
*Primary contacts are Emma and Keith
Per Minna: Dashboard needs to be accessible, with large print and text-to-speech alternatives.

## Project approvals and dependencies:
I need to make sure stakeholders have access to all datasets so they can explore the steps I’ve taken.\
Project goal: Explore trends in repeat callers

Details from Mr. Portone:
* Understand how often customers are calling customer support after their first inquiry; this will help leaders understand how effectively the team is able to answer customer questions the first time
* Provide insights into the types of customer issues that seem to generate more repeat calls
* Explore repeat caller trends in the three different market cities
* Design charts so that stakeholders can view trends by week, month, quarter, and year. 
  
 ## The deliverables and metrics:
* A chart or table measuring repeat calls by their first contact date
* A chart or table exploring repeat calls by market and problem type
* Charts showcasing repeat calls by week, month, and quarter

## Measure success:
The team’s ultimate goal is to reduce call volume by increasing customer satisfaction and improving operational optimization. My dashboard should demonstrate an understanding of this goal and provide stakeholders with insights about repeat caller volumes in different markets and the types of problems they represent. 
Other considerations:
In order to anonymize and fictionalize the data, the datasets the columns market_1, market_2, and market_3 to indicate three different city service areas the data represents. 

## The data also lists five problem types:
* Type_1 is account management
* Type_2 is technician troubleshooting
* Type_3 is scheduling
* Type_4 is construction
* Type_5 is internet and wifi

Additionally, the dataset records repeat calls over seven-day periods. The initial contact date is listed as contacts_n. The other call columns are then contacts_n_number of days since first call. For example, contacts_n_6 indicates six days since first contact. 
People with dashboard-viewing privileges: 
Emma Santiago, Keith Portone, Minna Rah, Ian Ortega, Sylvie Essa

## Questions:
* How often does the customer service team receive repeat calls from customers?
* What problem types generate the most repeat calls?
* Which market city’s customer service team receives the most repeat calls?


# Part 2

## Google Fiber datasets
By now, you are getting ready to take the next steps with your Course 2 end-of-course project. To work with the Google Fiber data, you will need to upload your data to the appropriate workspace. If you plan on using BigQuery or Dataflow, upload the files to your project space to JOIN them. Additionally, because this data is already clean, you can connect these datasets in Tableau directly and merge them there. 

Your interviewers have provided three CSV files: 

* [Market_1](https://docs.google.com/spreadsheets/d/1a9IKjkvOvYHRx84SyRdp4Sq81EzgeOZPufcRtrUcAIc/template/preview#gid=775366698)
* [Market_2](https://docs.google.com/spreadsheets/d/19CINdvAwp-2RF5pphkLywZLQJyJu66EOjX6CgrW32nA/template/preview#gid=2065220237)
* [Market_3](https://docs.google.com/spreadsheets/d/1K6X9ZhjWtbneBss7PQH7IobGCzQ5NzG1hxs1D-hbsZM/template/preview?resourcekey=0-q90E-1XwD8nkNSjs0Ws3-w)

Upload to BigQuery
First, navigate to your BigQuery console. Go to the BigQuery homepage or go directly to the console.
![BigQuery Console] 

The BigQuery homepage with the Go to console button

Click on the + ADD DATA button in the Explorer menu pane to open the Add Data menu. 

The Add Data menu in BigQuery

From here, select Local file to upload the CSV or Google Cloud Storage to choose the sheet from your personal Drive. However you add the file, you will need to fill out the necessary fields in the Create Table menu. If you haven’t already, the Create table menu will also prompt you to create a dataset to house this table.

Create table menu prompting user to CREATE NEW DATASET

Select CREATE NEW DATASET and name the dataset appropriately for this project. Leave the data location set to default. Once you have completed filling out this information, click Create Dataset. 

Now, finish filling out the information for your table. Name your table appropriately for your project and select CSV under file type. Finally, select Auto detect for the schema. Once done, select Create Table. The new table should appear under your dataset in the Explorer pane momentarily. 
