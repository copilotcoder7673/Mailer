# Mailer
A Simple Email Sender Api In NodeJS

### required parameters 
request and response body type : json

sender,
password,
recipient,
subject,
message

Example Code Snippet To Send Mail using Javascript fetch

```javascript
const apiUrl = "https://gmailapi-armanidrisi.vercel.app/api/mail/";

const requestBody = {

  sender: "yourmail@gmail.com",

  password: "yourpass",

  recipient: "receiver mail",

  subject: "subject",

  message: "msg"

};

fetch(apiUrl, {

  method: "POST",

  headers: {

    "Content-Type": "application/json"

  },

  body: JSON.stringify(requestBody)

})

  .then(response => response.json())

  .then(data => console.log(data))

  .catch(error => console.error(error));

```
