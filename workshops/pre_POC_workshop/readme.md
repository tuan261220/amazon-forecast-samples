# Amazon Forecast pre-POC Workshop - hands-on Bring Your own Data

In this workshop, you will get hands-on and learn how to use Amazon Forecast with your own data.  We will go through a complete data pipeline.  From raw data input - to training a model on that data - to generating inferences (forecasts) from the model - to exporting and visualizing the forecasts.  

This workshop is designed to accelerate customers doing an Amazon Forecast POC.  The architecture components will make experimentation and iteration of Forecast models easier for your POC project.  The components installed during the workshop can remain in your account after the workshop, so you can keep using these tools to perform experimentation with Forecast models.

By default, the installed AWS service components do not incur any cost when not in use.  

- [ ] Warning:  SageMaker is the only AWS service in this solution you need to take extra precautions about when not in use.  As installed, the Forecast solution will not incur cost.  However, if you do open a SageMaker Notebook, make sure to shut down all Notebook instances when not in use, otherwise SageMaker will keep charging, even when not in use.



### Day of workshop.  Typical agenda.

| **Start** | **End** | Who                      | **Activity**                                                 |
| --------- | ------- | ------------------------ | ------------------------------------------------------------ |
| 9:00a     | 9:30a   | Customer                 | Introductions, customer's Exec sponsor set the stage of the exact problem that is to be tackled and what success looks like for the POC engagement. |
| 9:30a     | 10:00a  | AWS                      | Slides - High-level overview of Amazon Forecast<br />[See Intro section of Amazon Forecast Cheat Sheet](https://github.com/aws-samples/amazon-forecast-samples/blob/master/ForecastCheatSheet.md) |
| 10:00a    | 10:30a  | AWS                      | Demo - Console demo of NYC taxi data. <br /> TODO: link 5min video |
| 10:30a    | 10:45a  | All                      | Discussion - mapping customer's data to the Forecast POC problem.  <br />[See Getting Started Best Practices](https://github.com/aws-samples/amazon-forecast-samples/blob/master/ForecastCheatSheet.md) |
| 10:45     | 11:00   | BREAK                    | 15min BREAK                                                  |
| 11:00a    | 12:00p  | AWS leading the customer | - Developers:  Suggest using Glue DataBrew, save TTS to S3.  TODO link 5min video<br />- Data Scientists: <br />- If data is Daily or Hourly - [use the regular DataPrep notebook](https://github.com/aws-samples/amazon-forecast-samples/blob/master/workshops/pre_POC_workshop/1.Getting_Data_Ready_nytaxi.ipynb) to save TTS to S3<br /> - If data is Weekly or higher - [use the weekly DataPrep notebook](https://github.com/aws-samples/amazon-forecast-samples/blob/master/workshops/pre_POC_workshop/1.Getting_Data_Ready_nytaxi_weekly.ipynb) to save TTS to S3 <br />- To launch Predictor using just TTS and AutoML using console. [See Getting Started Tutorial](https://github.com/aws-samples/amazon-forecast-samples/blob/master/ForecastCheatSheet.md)<br />- To launch Predictor using just TTS and AutoML using the solution:<br />- Edit the .yaml file<br />- Find the train/ folder of solution S3 bucket<br />- upload .yaml file in root of solution S3 bucket <br />- copy customer's S3 data in train/ folder |
| 12:00p    | 1:00p   | LUNCH                    | 1hr LUNCH<br />                                              |
| 1:00p     | 1:30p   | AWS                      | Overview Solution Architecture components, see https://github.com/aws-samples/amazon-forecast-samples/blob/master/workshops/pre_POC_workshop/install-forecast-solution.md |
| 1:30p     | 2pm     | AWS leading customer     | Evaluate Predictor (in console, using Query, and in QuickSight)<br />[See getting Started Tutorial](https://github.com/aws-samples/amazon-forecast-samples/blob/master/ForecastCheatSheet.md) |
| 2:00p     | 2:30p   | AWS leading customer     | Start Discussion:  Iterate on Dataset and Models <br /<br />[See Iterating Models / What-if Best Practices](https://github.com/aws-samples/amazon-forecast-samples/blob/master/ForecastCheatSheet.md)<br /> |
| 2:30p     | 2:45p   | AWS                      | Summarize what was learned                                   |
| 2:45p     | 3:15p   | Customer                 | Presentation to Exec Sponsor what they learned, accomplished, and possible next steps |
| 3:15p     | 3:30p   | END WORKSHOP             | Answer Questions                                             |
