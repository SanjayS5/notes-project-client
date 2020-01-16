### Project Name: Parchment – A simple personal journal
### Project Description: 

This application allows a user to sign up, login, and create their own notes or personal journal entries. The user will be able to create a new entry, along with the ability to edit and delete those entries. 

### Architecture Diagram

![Screen Shot 2020-01-16 at 1 13 35 pm](https://user-images.githubusercontent.com/34014570/72482375-5dceb600-3862-11ea-8d14-aebb496065ff.png)


### Tech Stack: 

•	React
•	React Router
•	React-Bootstrap
•	HTML
•	Python
•	AWS Cognito
•	AWS Amplify
•	AWS API Gateway
•	AWS Lambda
•	AWS DynamoDB
•	Serverless Framework 
•	GitHub

### How I built the application:

I started by developing the API for Parchment on AWS. I created the lambda functions for all the main CRUD operations, linking them to DynamoDB and API gateway. Once these were tested and determined to be working correctly, I built the frontend user interface in React and linked the API to it. Following this, I uploaded the React app and ensured that it is now live on the Internet. 

The frontend was built utilising a tutorial: https://serverless-stack.com/chapters/create-a-new-reactjs-app.html

Most of the code is from there, however I did need to learn React to modify the code to my needs. 

### How to run the application: 

You can access the application through this link:
http://parchment.com.s3-website-ap-southeast-2.amazonaws.com/

### How to test the application:

Tests can be run using the Serverless Framework. For example:
$ serverless invoke local --function create --path mocks/create-event.json

This code invokes the “create” function locally, retrieving the test values from the “mocks” directory. 

### Software tools used:

•	VS Code
•	AWS Console

### User Flow:


![Screen Shot 2020-01-16 at 11 03 43 am](https://user-images.githubusercontent.com/34014570/72476094-328f9b00-3851-11ea-9e46-d57a7c189b13.png)

 
Login: The user would first have to sign up, then login from this page. 

![Screen Shot 2020-01-16 at 10 57 42 am](https://user-images.githubusercontent.com/34014570/72475997-efcdc300-3850-11ea-842c-7effc0dca7de.png)

 Homepage: The homepage, utilising the GET request to list all the results from DynamoDB. From here, the user could click create a new note and be taken to the page below.

![Screen Shot 2020-01-16 at 10 58 16 am](https://user-images.githubusercontent.com/34014570/72476013-f9572b00-3850-11ea-8d93-d44bd02c142c.png)
 
Creating a new note: The user can create the note, click “Create” and they will be redirected the homepage.

![Screen Shot 2020-01-16 at 10 58 29 am](https://user-images.githubusercontent.com/34014570/72476017-fb20ee80-3850-11ea-9ded-8597e86f73b2.png)

Editing or deleting an existing note: Alternatively, the user could decide to click on an existing note and chose to edit it or delete it from this page. The user will then be redirected to the homepage.  

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).
