# Fake person generator project done with UiPath Studio

## Process
- Program asks user to choose the folder on which the excel file will be saved
- Then it asks to write a name for the file.
- Lastly the number of fake people the robot fetches from the website.

## Robot
- After the user input, the robot opens the browser in url "https://www.fakepersongenerator.com/"
- The robot saves the persons contact information in variables and adds them to the datatable.
- Once the webpage throws a captcha in about 13 fetches, the robot just opens the page again.
  - (This will take few tries, but eventually will navigate to the page)
- When wanted number of fake contact information has been collected, the robot closes the browser and 
  inserts the data to an excel file initiated before.
  - Robot will also ask if the user would like to have the data as JSON file. If confirmed, the JSON file 
    will be created in the same path with same name as the Excel file.
  
## Learning
- During this assignment I learned much about error handeling, selectors, converting data to JSON format and excel file tools in UiPath.
- I also learned how to use GIT integration in UiPath.
