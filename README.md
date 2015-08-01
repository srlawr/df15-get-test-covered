# df15-get-test-covered
The trailhead quick start project for geting your first test class up and running

# Intro

Automated testing is not just a good idea to keep your code and projects stable and reliable, it is also a requirement of the Salesforce release process. This project will provide you with a short Apex service class, which you will then go ahead and write a test class for, to achieve 100% code coverage.

# Steps

## Step 1 - Create some code to cover
Quickly complete the following steps to create a class, which contains XYZ lines of testable code.

1. From your developer edition, click on your name in the top right corner, and launch the developer console from the drop-down menu.
2. In the developer console, click "File" and then use "New" to create a new Apex Class.
3. Call the class ""
4. Copy and paste the following code into the file, and save it. You should see "Saving" in the title briefly, and then the class will be created in your org.

Now we have some code in place, if you switch to the "Test" tab in the Developer console, you should see we have 0% coverage of this class, so it's time to do something about that.

## Step 2 - Create a test class and setup your test conditions

1. Go back to "File" and use "New" to create another class. Call this one "test".
2. In Salesforce we typically use @Annotations to indicate test classes and methods. Paste the following into your new test class to get the ball rolling


The @isTest declaration at the top tells Salesforce this is a test class, so it will appear in the relevant lists. Test code does not contribute to your overall Apex usage limit, so writing plenty of tests will not hinder you.

Test classes do not have access to existing data in your Salesforce org, so the @testSetup method is called before each test method is run to insert our pre-defined test data. In this case we need to insert a XY and Z

Now, paste this first test mehtod into the class, which will test that X and Y are true when Z happens.


Once saved, go to "Test" in the developer console top menu, and select "New Run". Pick the test class and move it over to the right hand list, and click "Run". At the bottom of the page you should see your test class queued up (possibly with an orange circle). Eventually it will run and be marked with a green tick to indicate it has passed. You may wish to click around to see the details of the results.

Go back to the tab containing our original code, and at the top click the drop down to show the code coverage. You can see we have achieved AA%, lets got back to the test class and complete this testing.

Paste the following method into the the test class alongside the first. You can see that this method now tests A and B.

Save the file and go to "Test" in the top menu and "Re-run". Once the test has been queued and executed, if you return to the original code, you should see you now have 100% coverage between these two test methods, and your work is complete!

# Summary

Writing test classes and methods is really simple and quick in Salesforce, and using the @testSetup annotation, you can be sure they will work as expected when run because the data over which they run is specifically defined in the test class itself.

Running tests and seeing their effects in the Developer Console is an effective way of managing and monitoring your coverage levels.

# Resources
