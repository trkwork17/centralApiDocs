# API Quickstart

<!-- This document describes how to start using your API: authorization, authentication, accessing API resources. -->
In this section, you'll find a step-by-step guide to quickly start using the API.

## Prerequisites

List any prerequisites or dependencies that users need to have in place before they can start using the API.

* Pre-requisite one
* Pre-requisite two

## Authentication

To authenticate with the API, you need to log in, the options are 
  
 * **Agent**
 * **staff**
 * **sub agent**
 * **Admin**
 * **Super Admin**

To get the tokens.

## Making Your First Request

Provide a simple example of making a request to one of the API's endpoints. Clear and concise code snippets.

```http
POST /api/v1/agent/create_staff HTTP/1.1
Host: https://quickticketsb2b-nodejs.de.r.appspot.com
Authorization: Bearer YOUR_ACCESS_TOKEN
```
 * Request Body
```json
    {
  "name": "Agent Staff 2",
  "email": "agentstaff2@gmail.com",
  "password": "12345678",
  "confirmPassword":"12345678",
  "designation": "Admin",
  "phone": "+880163456756",
  "role": "admin"
}
```
## Response Handling
Explain how to handle the API responses, including parsing JSON data and handling errors.

* Response

**Status 200 OK**

```json
       {
  "success": true,
  "message": "Staff successfully created",
  "data": {
    "id": "29100625ac7e48a9a7b4439bd09b719f",
    "uid": 9,
    "staffId": "QTS1009",
    "agentId": "c1d00d32551511eea7051831bf245c65",
    "name": "Agent Staff 2",
    "email": "agentstaff222@gmail.com",
    "phone": "+880163456756",
    "designation": "Admin",
    "role": "admin",
    "status": "active",
    "created": "2023-11-20T10:54:32.000Z",
    "createdBy": "agent",
    "subagentId": null,
    "nidCopy": null
  }
}
```


## API Usage Tips
Offer tips and best practices for using the API effectively and efficiently.

## Next Steps
Suggest what users can do next, such as exploring more endpoints or integrating the API into their applications.