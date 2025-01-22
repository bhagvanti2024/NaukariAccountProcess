# NaukariAccountProcess
Here's a description of your Selenium WebDriver program for automating interactions with Naukri.com's login, job recommendation, and logout functionalities. The program is structured using the Page Object Model (POM) and TestNG framework, ensuring a modular and maintainable codebase.

Description:
NaukariAccountClass (Page Object Model Class):

This class represents the elements and actions for the Naukri.comaccount page.

Attributes:

WebDriver driver: The WebDriver instance for browser interactions.

Actions act: The Actions class instance for advanced user interactions.

WebElement login: Locator for the login button.

WebElement usernamename: Locator for the username input field.

WebElement password: Locator for the password input field.

WebElement loginbtn: Locator for the login button.

WebElement job: Locator for the Jobs section.

WebElement recjob: Locator for the Recommended Jobs section.

WebElement profile: Locator for the profile icon.

WebElement logout: Locator for the logout button.

Methods:

public NaukariAccountClass(WebDriver driver1): Constructor to initialize WebDriver and PageFactory elements.

public void Loginfun(): Method to perform login action.

public void JobReco() throws InterruptedException: Method to interact with the Jobs section and click on Recommended Jobs.

public void Logout(): Method to perform logout action.

NaukariAccountTest (TestNG Test Class):

This class contains the test setup and test methods using the TestNG framework.

Attributes:

WebDriver driver: The WebDriver instance for browser interactions.

NaukariAccountClass home: Instance of the POM class.

Methods:

@BeforeClass public void BeforeClass(): Method to set up the WebDriver and initialize the POM class.

@BeforeMethod public void BeforeMethod(): Method to navigate to the Naukri.comURL and perform the login action.

@Test public void Jobrecommendation() throws InterruptedException: Test method to verify the Recommended Jobs functionality.

@AfterMethod public void AfterMethod(): Method to perform the logout action.

@AfterClass public void AfterClass(): Method to close the WebDriver instance.
