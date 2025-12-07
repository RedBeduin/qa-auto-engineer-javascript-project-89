### Hexlet tests and linter status:
[![Actions Status](https://github.com/RedBeduin/qa-auto-engineer-javascript-project-89/actions/workflows/hexlet-check.yml/badge.svg)](https://github.com/RedBeduin/qa-auto-engineer-javascript-project-89/actions)

[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=RedBeduin_qa-auto-engineer-javascript-project-89&metric=coverage)](https://sonarcloud.io/summary/new_code?id=RedBeduin_qa-auto-engineer-javascript-project-89)

[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=RedBeduin_qa-auto-engineer-javascript-project-89&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=RedBeduin_qa-auto-engineer-javascript-project-89)

### The testing of the chat bot widget
This project has purpose to test the registration form and the widget of the chat bot of the educational platform.

### Automatical tests directory
All files with automatical tests of the widget and application are stored in the \_\_tests\_\_ folder.

### How to copy the project to your PC
To copy this project to your PC, open Ubuntu, type in the command line
```
git clone https://github.com/RedBeduin/qa-auto-engineer-javascript-project-89.git
```
and rename the repository of the project if you want.

### How to open the application and the window with registration form and chat bot widget that are tested in the project
To open the application, open Ubuntu on your PC, move to the directory of the project and type in the command line
```
npm run dev
```
to launch the application,
then type
```
o
```
to open the window with the registration form and the chat bot widget.

### Interaction with the registration form and chat bot widget
Then you can fill the registration form and click at checkbox field, send the filled form, type the buttons in the chat bot interface or close the window with the registration form and chat bot widget.

### Interaction with the application in Ubuntu via command line
Then you should type in the command line
```
h
```
to see help information
OR
```
q
```
to exit the application.

### Exploring the test directory and the test files 
Then you can type in the command line
```
cd __tests__
```
to move to the directory with tests
and type
```
ls -a
```
to see the structure of the directory.
To see the test files it is better to use the code redactor program.

### Technologies that are used in the project
* For the project **application with help information, registration form and chat bot widget** is used. This is the application of the educational platform that was not developed in this project. 

* In this project an automatical testing of this application, following the technology **"Page Object Model"(POM)**, was written in two files:
  * app.spec.jsx - testing of the application
  * widget.spec.jsx - testing of the chat bot widget  
**Page Object Model(POM)** is a pattern of projecting for automatization of testing of web-applications. In POM each web-page or massive part of the page is represented as class. This class contains methods which give opportunity to interact with elements of the page such as buttons, input fields etc. Main purpose of the POM is to separate logic of the testing from logic of the interaction with elements of the page.

* In the project **coverage of the edge cases** was realized

* **Testing of interaction between the user and the application** was developed in \_\_tests\_\_/pages directory files with page models and in \_\_tests\_\_ directory files with test units for Application and Widget. 

* In the conclusion it is important to mention, that 
  * **the testing of integration of the widget with the application**,
  * **the model of the widget**,
  * **the model of the application**  
were made in the project. 

* Also **CI/CD** was used by linking the project with SonarQube space to check the quality and the correct work of the project.  
**CI/CD (Continuous Integration/Continuous Delivery or Deployment)** - is a metodology of development of program software, that speeds up the release of the product and improves the quality of the product through the automatization of the assembly processes, the testing and the deployment of the code. Continuous Integration (CI) automatizes the merge of the code written by developers in the shared repository with the automatical testing as the following step. Continuous Delivery (CD) prepares the code for release through automatical deployment of the code in the testing space for the subsequent manual launch to production and Continuous Deployment (another interpretation of CD) automatically delivers this code to the users.

### Important data files in the \_\_fixtures\_\_ directory
In the \_\_fixtures\_\_ directory file with example steps of interaction with chat bot(steps.js), file with example of incorrect interaction with chat bot(error-steps.js) and vault with phrases of chat bot(text-set.js) were written.

### Directory with constants
All text constants that are used in the project, except Chat Bot Phrases, are stored in the \_\_tests\_\_/utils/constants.js file that is exported(each constant is exported separately) and used in another files of project through import of this file. Chat Bot Phrases are stored in the \_\_fixtures\_\_/text-set.js file that is also exported(the constant textSet is exported) and also used through import of the constants in another files of the project that require these constants. This separation into two files was made to divide the text constants of the project into two types - in constants.js: labels, text contents of the buttons and text content of the title of the modal window and in text-set.js: the Phrases of the Chat Bot. 
