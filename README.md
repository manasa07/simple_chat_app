#DESCRIPTION

This project creates a full-stack platform specific to run Automated scripts for IDS.

#Pre-Requisites

Eclipse IDE, Selenium-server-standalone-3.7.1.jar, Download testing-6.8.5.

Configuration : Ensure the project build paths are correctly set-up. Selenium-server-standalone-3.7.1.jar is must.
URL, environment, browser-name in [sonnettest.properties.( https://gitlab.pnmac.com/qa-automation/IDS/ids-automation/blob/master/sonnettest.properties)



Building The Project :
Keep all the Objects Page-wise, For all Pages keep in a Package, All re-usable methods and common methods keep in Base class, Accordingly the Framework structure has to be designed.
All Base methods for all actions on UI Elements are present in SonnetSelenium.
Reporting purpose there is third-party tools ‘Extent Reports’.
Write All Page Objects respective to pages in PageObjects.java and to drive the Test, Create an object of that class in respective test class and use TestNG Annotations.
@Before Class : Call the browser, Navigation, Report Title
@Test : Call all the methods here to run the Tests, Right-click on the Editor and Run as TestNG Test.
@After Class : Flush and Quit the driver.
Always try to keep the code simple, readable and reusable, Write Generic methods according to Test Scripts specific so that there is Data Redundancy, It should be optimized.

CVS : Generate SSH keys and configure first, Create a folder in Gitlab, Now daily Commit your day-today work in separate branch and push the code through GitBash commands or through Git Extensions Client, to GitLab, So the concerned Person will review the code and merge it with Master.
