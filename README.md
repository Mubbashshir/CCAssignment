# CCAssignment

                       Selenium using Page Object Model and BDD



Summary: 6 Scenarios have been created using page object model&BDD. Log4J is used for capturing logs&cucumber reports for capturing results. Given below are the details


Main Java Classes:

	Home.Java: Contains all the elements of  https://www.costcutter.co.uk/location-finder/  page and related methods in java.
	StoreFinderPage.Java: Contains all the elements of https://www.costcutter.co.uk/location-finder/results/ and related methods in java. 
	TestBase.Java: Contains all the details of various driver declaration and initialization. 
	Test Runner.Java: It facilitates running the of selenium scripts and has path for 
	cucumber feature file and steps definition file 
	StorepageTestSteps.Java: This class has coding for various step definitions for executing the selenium scripts. 


Cucumber Feature File: 

	Cucumber Feature File: The name of the feature file which we are using is CostcutterStorePage.feature which has all the scenarios in Gherkin language and they are linked to step definition file(StorepageTestSteps.Java) which will execute the test steps defined in feature file using java and selenium. 

Log files& Cucumber Report: 

	Log4J: This is used for logging purposes and also helps with trouble shooting to verify the actual cause of failure. 

	Log4J Location: Its located in MainProjectName/src/test/java.


	Configuration: Currently the logs are created at C:\Setups\Logs if you want to use the same folder structure please create these two folder under C drive or change the folder location in log4J.properties.  

	Cucumber Report: The Cucumber report helps to report on Selenium scripts test status such as number of scripts passed or failed. The location of this report is at
Main Project Name/target/site/cucumber-pretty/index.html


 Results: Out of 7 Scenarios, 3 are planned to fail as I have given invalid inputs. I 
 have used soft assertions to ensure the failed results are shown in Cucumber report and these assertions unlike hard assertions will not stop execution of later steps in step definition file.  
