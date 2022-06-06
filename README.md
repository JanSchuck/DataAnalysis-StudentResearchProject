# Student research project

In this student research project i did during the "Datenanalyse in der Praxis" course i scraped job informations from Indeed
and tried to find out which skills are expected the most as a Data Analyst. 

## Webscraper
For the webscraping i am using Selenium because it provides features for interactions with the website.
This is mandatory for clicking through cookie windows and to click through different job offers and "next page".

The website investigation aspect is not to be neglected. It was quite difficult to find a way to click through the list of job offers.
I solved the problem by getting the id of every job and later build the XPATH with these id's to click each job so that the full desciption appears.

When the description appears you have to switch to the job frame to get the data. When done you have to switch back to the default frame.

These are the informations that i scraped:
job_id, job_title, company_name, company_location, job_type, job_Description, date_time

I searched for Data Analyst in Germany.

The Webscraper can also be used for different jobs and locations.

## Analysis
To find out which skills are expected the most you "explode" the descriptions. This means you break down the description to its single words.
Than you create a list of skills that you are looking to investigate. In this case:

"excel" , "python" , "r" ,"matlab", "ai", "ki", "mysql" , "linux", "c",
"visio", "java", "javascript", "vba", "powerpoint", "github", "git", "gitlab",
"sql", "mysql", "sqlight"

The most expected skill was SQL which occured in 40% of the job offers followed by python with 31% and Excel with 18%

| keywords      | counts        | percentage    |
| ------------- | ------------- | --------      |
|sql            |       123     | 40.196078     |
|python         |        94     | 30.718954     |       
|excel          |        54     | 17.647059     |     
|r              |        49     | 16.013072     |
|powerpoint     |        20     | 6.535948      |
|java           |        19     | 6.209150      |
|javascript     |        15     | 4.901961      |
| git           |        9      | 2.941176      |
| vba           |        9      | 2.941176      |
| c             |        9      | 2.941176      |
| sql           |        123    | 40.196078     |
| python        |        94     | 30.718954     |
| excel         |        54     | 17.647059     |
| r             |        49     | 16.013072     |
| powerpoint    |        20     | 6.535948      |
| java          |        19     | 6.209150      |
| javascript    |        15     | 4.901961      |
| git           |        9      | 2.941176      |
| vba           |        9      | 2.941176      |
| c             |        9      | 2.941176      |

The best location for finding a Data Analyst job is Berlin followed by homeoffice and München

| location              | counts        |       
| -------------         | ------------- | 
| berlin                |         37    |
| homeoffice            |        16     |
| münchen               |        14     |
| hamburg               |        11     |
| frankfurt_am_main     |        9      |

When it comes to the question of Python vs R. Python clearly was more asked:

|    keywords | counts | percentage
| ------------- | ------------- | --------      |
|    python |     94 |  27.089337
|        r |     49 |  14.121037

