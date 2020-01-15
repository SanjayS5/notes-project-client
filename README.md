Project Name: Parchment – A simple personal journal
Project Description: 

This application allows a user to sign up, login, and create their own notes or personal journal entries. The user will be able to create a new entry, along with the ability to edit and delete those entries. 

Tech Stack: 

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

How I built the application:

I started by developing the API for Parchment on AWS. I created the lambda functions for all the main CRUD operations, linking them to DynamoDB and API gateway. Once these were tested and determined to be working correctly, I built the frontend user interface in React and linked the API to it. Following this, I uploaded the React app and ensured that it is now live on the Internet. 

The frontend was built utilising a tutorial: https://serverless-stack.com/chapters/create-a-new-reactjs-app.html

Most of the code is from there, however I did need to learn React to modify the code to my needs. 

How to run the application: 

You can access the application through this link:
http://parchment.com.s3-website-ap-southeast-2.amazonaws.com/

How to test the application:

Tests can be run using the Serverless Framework. For example:
$ serverless invoke local --function create --path mocks/create-event.json

This code invokes the “create” function locally, retrieving the test values from the “mocks” directory. 

Software tools used:

•	VS Code
•	AWS Console

User Flow:

 
Login: The user would first have to sign up, then login from this page. 


 Homepage: The homepage, utilising the GET request to list all the results from DynamoDB. From here, the user could click create a new note and be taken to the page below.


 
Creating a new note: The user can create the note, click “Create” and they will be redirected the homepage.
 Editing or deleting an existing note: Alternatively, the user could decide to click on an existing note and chose to edit it or delete it from this page. The user will then be redirected to the homepage.  





This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (Webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `npm run build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify
