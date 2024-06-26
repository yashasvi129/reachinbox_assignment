# reachinbox_assignment
#Deployed Links

frontend : https://reach-inbox-assignment.vercel.app/

Backend : https://documenter.getpostman.com/view/31971527/2sA35D43FE

API documentation build with postman documentation - https://documenter.getpostman.com/view/31971527/2sA35D43FE


#technologies used:

Node.js
Express.js
OpenAI
Google APIs
Microsoft Graph API


#npm packages used:

dotenv
Axios
bullMQ
google-auth-library
ioredis
@microsoft/microsoft-graph-client
@azure/msal-node



Installation setup

Clone the repository to your local machine
git clone https://github.com/shraddha-gawde/reachInbox-assignment.git


Navigate to the root directory of the project directory :
cd server


Run npm install to install all the dependencies


Create a .env file in the root directory with the same IDs as specified in the documentation.
Running the server



To start the server, run the following command in your terminal
npm start
This will start the server at localhost:5000 (or whatever port you have specified). or we can use backend deployed link also.



To start the worker.js file, run the following command in your terminal
npm run server



API Endpoints
For Google's OAuth2.0:
https://reachinbox-assignment-4rf9.onrender.com/auth/google - GET for google authentication
https://reachinbox-assignment-4rf9.onrender.com/api/mail/userInfo/:email - GET request to view user profile
https://reachinbox-assignment-4rf9.onrender.com/api/mail/allDrafts/:email - GET request to view all drafts mail.
https://reachinbox-assignment-4rf9.onrender.com/api/mail/read/:email/message/:message - GET request to read a specific email(using id).
https://reachinbox-assignment-4rf9.onrender.com/api/mail/list/:email - GET request to get a list of mails.
https://reachinbox-assignment-4rf9.onrender.com/api/mail/sendMail - POST request send mail with label.
{
    "from":"sendersmail@gmail.com",
    "to":"recieversmail@gmail.com",
    "label":"interested/not-interested/more-information"
}
https://reachinbox-assignment-4rf9.onrender.com/api/mail/sendone/:id - POST request to send a single mail for particular ID.
{
    "from":"sendersmail@gmail.com",
    "to":"recieversmail@gmail.com"
}
https://reachinbox-assignment-4rf9.onrender.com/api/mail/sendMultiple/:id - POST request to send a single mail for particular ID.
{
   "from":"sendersmail@gmail.com",
   "to":["demo@gmail.com","demo@gmail.com", "demo@gmail.com"]
}
