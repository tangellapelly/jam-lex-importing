* Login to your aws account.
* Once you login, search for Lex in the aws console and click on it to open.

* Once you have Lex, go head and import the _gasStationsNearBy_Bot_LEX_V11.zip_ from **Actions >> Import**

* Now, go back to the aws console again to search for Lambda and click on to lunch it.

* In the Lambda dashboard you need click on the **Create Function** button to create the Lambda function. In the next screen you will need to give a name for your function, go ahead and fill in "gasStationsNearBy" then click on the **Create Function** button in the bottom of the page. This will create the lambda function for you.

* In the next screen your Lambda function will be displayed, scroll to the **Function Code** section and from the **code entry type** dropdown select  **upload a .zip file** to upload the function. 

* Once you uploaded the .zip file, click on the **Save** button top right to save it.

* Now, you see the lambda code in the **Function Code** section. Its grab the APP_ID and APP_CODE from the AWS Market Place to setup the environment variables for our Lambda.

* Once you have the APP_ID and APP_CODE, go ahead and setup the environment variables from the **Environment Variables**.

* You need to test the function to make sure its working properly. You need to configure a test event from dropdown towards the left of the **Test** button on the top right. You need to copy the code from the _Lambda-Test-case.json_ to finish the **Configure test event**.

* Once you setup the test event, go ahead and click on the **Test** button to make sure everything working fine.

* Now, go back to the Lex dashboard and select the **gasStationsNearBy** Bot that you have imported. Now, you need to  integrate **gasStationsNearBy** Lambda from the **Fulfillment** section.

* Finally, go ahead to and click on the **Build** on the top right to test your bot.

