# Serenity-Selenium-Sample

[Serenity](http://www.thucydides.info/docs/serenity/) Integration with [LambdaTest](https://www.lambdatest.com).

![LambdaTest Logo](https://www.lambdatest.com/images/logo.svg)

<img src="http://www.thucydides.info/docs/serenity/images/serenity-logo.png" height = "50">


## Prerequisites for running tests using Serenity automation framework :

## Environment Setup 

### 1. Java Installation
   
   i.   For Windows :
   
   You can download Java for Windows from [here](http://www.java.com/en/download/manual.jsp)
   
   Run the installer and follow the setup wizard to install Java.
   
   create a new JAVA_HOME environment variable and set variable value as path value to JDK folder.
   
   #### This is Windows environment variable location :
   Control Panel > All Control Panel Items > System > Advanced system settings > Environment Variables
   
   ![altext](https://github.com/keshavissar001/selenide-testng-sample/blob/keshavissar001-patch-1/Img1.png)
   
   ii. For Linux :
   
   use this command :
   ```
   sudo apt-get install openjdk-8-jre
   ```
   iii. For Mac
   
   Java should already be present on Mac OS X by default
   
   ### 2. Maven Installation
   
   Install Maven from [here](https://maven.apache.org/install.html)
   
### 3 Setup

   You can download the file. To do this click on “Clone or download” button. You can download zip file.
   
   Right click on this zip file and extract files in your desired location.

   Go to “selenide-testng-sample-master” folder and copy its path.
   Open command prompt and run :
   
    cd <path> (that you have copied)
    
    (please ignore "<" , ">" symbols)
    

![altext](https://github.com/keshavissar001/images/blob/master/SerenityPath.png)


	To clone the file, click on “Clone or download” button and copy the link.

	Then open the command prompt in the folder you want to clone the file. Run the command:

      git clone <paste link here> 


 LambdaTest Credentials
   Set LambdaTest username and access key in environment variables. It can be obtained from [LambdaTest Dashboard](https://automation.lambdatest.com/)    
    example:
    
   For linux/mac
   
    ```
    export LT_USERNAME="YOUR_USERNAME"
    export LT_ACCESS_KEY="YOUR ACCESS KEY"

    ```
    
    For Windows
    
    ```
    set LT_USERNAME="YOUR_USERNAME"
    set LT_ACCESS_KEY="YOUR ACCESS KEY"

    ```

Install dependencies `mvn install`

You can set environment variables or update `serenity.properties` file with your [LambdaTest Username and Access Key](https://automation.lambdatest.com)

## Running your tests


- To run a single test, run 

`mvn verify -P single`

![altext](https://github.com/keshavissar001/images/blob/master/SerenitySingleResult1.png)

![altext](https://github.com/keshavissar001/images/blob/master/SerenitySingleResult2.png)

![altext](https://github.com/keshavissar001/images/blob/master/SerenitySingleResult3.png)

- To run parallel tests, run `mvn verify -P parallel`

Know how many concurrent sessions needed by using our [Concurrency Test Calculator](https://www.lambdatest.com/concurrency-calculator?ref=github)


## Notes
* You can view your test results on the [LambdaTest Automate dashboard](https://automation.lambdatest.com)
* You can export the environment variables for the Username and Access Key of your LambdaTest account
  
##  Testing Locally Hosted or Privately Hosted Projects

To help you perform cross browser testing of your locally stored web pages, LambdaTest provides an SSH(Secure Shell) tunnel connection with the name Lambda Tunnel. With Lambda Tunnel, you can test your locally hosted files before you make them live over the internet. You could even perform cross browser testing from different IP addresses belonging to various geographic locations. You can also use LambdaTest Tunnel to test web-apps and websites that are permissible inside your corporate firewall.

* Set tunnel value to True in test capabilities
> OS specific instructions to download and setup tunnel binary can be found at the following links.
>    - [Windows](https://www.lambdatest.com/support/docs/display/TD/Local+Testing+For+Windows)
>    - [Mac](https://www.lambdatest.com/support/docs/display/TD/Local+Testing+For+MacOS)
>    - [Linux](https://www.lambdatest.com/support/docs/display/TD/Local+Testing+For+Linux)

After setting tunnel you can also see the active tunnel in our LambdaTest dashboard:


![tn](https://github.com/Apoorvlt/test/blob/master/tn.PNG)

 ### Important Note:
 Some Safari & IE browsers, doesn't support automatic resolution of the URL string "localhost". Therefore if you test on URLs like "http://localhost/" or "http://localhost:8080" etc, you would get an error in these browsers. A possible solution is to use "localhost.lambdatest.com" or replace the string "localhost" with machine IP address. For example if you wanted to test "http://localhost/dashboard" or, and your machine IP is 192.168.2.6 you can instead test on "http://192.168.2.6/dashboard" or "http://localhost.lambdatest.com/dashboard".


## Notes
* You can view your test results on the [LambdaTest Automation Dashboard](https://www.automation.lambdatest.com)
* To test on a different set of browsers, check out our [Capabilities Generator](https://www.lambdatest.com/capabilities-generator)

## About LambdaTest

[LambdaTest](https://www.lambdatest.com/) is a cloud based selenium grid infrastructure that can help you run automated cross browser compatibility tests on 2000+ different browser and operating system environments. LambdaTest supports all programming languages and frameworks that are supported with Selenium, and have easy integrations with all popular CI/CD platforms. It's a perfect solution to bring your [selenium automation testing](https://www.lambdatest.com/selenium-automation) to cloud based infrastructure that not only helps you increase your test coverage over multiple desktop and mobile browsers, but also allows you to cut down your test execution time by running tests on parallel.
  
## Additional Resources
* [SeleniumHQ Documentation](http://www.seleniumhq.org/docs/)
* [Serenity Documentation](http://thucydides.info/docs/serenity-staging/)
* [LambdaTest Documentation](https://www.lambdatest.com/support/docs/getting-started-with-lambdatest-automation/)
