Hi and welcome to the Jam Lounge Module for HERE Technologies. Today you will walk through creating your own Lex Chatbot that uses the HERE Places API to find all the Gas Stations around at a GPS position.

Once you get setup, your mission is to convert this Gas Station chatbot into a Coffee Shops chatbot that can then return all the Coffee Shops near the Venetian hotel!

// Setup

Below are the getting started instructions that will walk you through the process of signing up for the HERE AWS Marketplace listing as well as configuring Lex and finally creating a Lambda to handle the chat requests.

# Phase 0 - Sign up for the HERE Marketplace Listing & download the assets from the Jam Lounge Module.
0. Head over to the HERE Marketplace listing and using your personal AWS credentials sign up for the HERE Marketplace listing.  After this you will be able to grab the HERE App ID and complete the challenge below. It is free to sign up and no credit card is required,

# Phase 1 - Creating the Lex Chatbot Stub
1. Login to your AWS account provided by the AWS Jam Lounge.
2. Once you login, search for Lex in the AWS console and click on it to open.
3. Once you have Lex, go head and import the _gasStationsNearBy_Bot_LEX_V11.zip_ from **Actions >> Import**

# Phase 2 - Setting up a Lambda to communicate with the HERE API's.
4. Now, go back to the AWS console again to search for Lambda and click on to launch it.
5. In the Lambda dashboard you need click on the **Create Function** button to create the Lambda function. In the next screen you will need to give a name for your function, go ahead and fill in "gasStationsNearBy" then click on the **Create Function** button in the bottom of the page. This will create the lambda function for you.
6. In the next screen your Lambda function will be displayed, scroll to the **Function Code** section and from the **code entry type** dropdown select  **upload a .zip file** to upload the function. 
** When prompted select the "Lambda-gasStationsNearBy.zip" from your downloaded assets.
7. Once you uploaded the .zip file, click on the **Save** button top right to save it.
8. Now, you see the lambda code in the **Function Code** section. Grab your APP_ID and APP_CODE from the <a href="https://developer.here.com">HERE Developer Portal</a> to setup the environment variables for our Lambda. 
9. Once you have the APP_ID and APP_CODE, go ahead and setup the environment variables from the **Environment Variables** section.

# Phase 3 - Testing that your Lambda is setup and working correctly
10. You need to test the function to make sure its working properly. You need to configure a test event from dropdown found towards the left of the **Test** button on the top right. You need to copy the code from the _Lambda-Test-case.json_ to finish the **Configure test event**.
11. Once you setup the test event, go ahead and click on the **Test** button to make sure everything working fine.

# Phase 4 - Wiring up your Lambda to your Lex Chatbot
12. Now, go back to the Lex dashboard and select the **gasStationsNearBy** Lex Chatbot that you have imported. Now, you need to integrate **gasStationsNearBy** Lambda from the **Fulfillment** section.
13. Finally, go ahead and click on the **Build** on the top right to test your bot.

# Phase 5 - Test your ChatBot
14. Assuming your Chatbot can build correctly, please copy and paste this string to test the functionality.  
** "gas stations near 12.972442,77.580643"

# Phase 6 - Now Convert your Chatbot into a Las Vegas Nevada, Coffeeshops-finding Chatbot
15. To complete your challenge you will need to convert the chatbot and then report back on the coffee shops around the Venetian hotel in Las Vegas, Nevada USA.
