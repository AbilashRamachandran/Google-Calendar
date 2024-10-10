# Google-Calendar
1. How to set up and run your automation?

	-> Install UiPath studio in your local machine
	-> Open the required main.xaml file in UiPath studio
	-> Credentials for Google calendar is saved as assets in UiPath Orchestrator(in order to run this xaml file need to setup your login 	   credentials in assets
	-> Click on Run button from Ribbon tab

2. Explanation of approach and design :
	
	-> This process is to automate the google calendar, get the events for the current month and export as an excel summary report.
	-> The entire process is designed with exception handling mechanism using Try Catch and Retry scope.
	-> Exceptions has been logged, in order to easily identify the errors occurred during the run, if any.
	Process step:
		1. Login to Google calendar
		2. Extracting all events for the current month
		3. Data manipulation has been done using Regex and LINQ for the creation of required final summary report
		4. Closing chrome application.		
