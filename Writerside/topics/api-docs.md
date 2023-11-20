# API Overview

<!-- This document provides an introduction into your API. -->

## Introduction

The Central API with Node.js and Express.js is a frontend-friendly serverside that handles user operations and
provides optimal routes.

## What you can do using <API name>

In the API, there are very few routes that are free like login forgot, reset password, all other  
routes to access them you should be an authorized user.There are two parts of the API one is Admin, although
you are not able to access it until you are an admin or the super admin creates your profile, so you can create
an account as agent then one of us admin approve your account then you can play your own games like create own staff
sub-agent approve them

## Authentication

The authentication methods based on express-JWT approach which blocks unauthorized access to user in route level
for free routes will not be required validation for private routes must pass the validation protocols even the 
super admin can't use agent or admin route to perform those operation super admin must perform through own route
and for password store use of argon2 because others like bcryptJs can only hash less than 70 worlds and argon2 not.
and requirements the API.

## Base URL

**Live URL** = [**https://quickticketsb2b-nodejs.de.r.appspot.com/**](https://quickticketsb2b-nodejs.de.r.appspot.com/)

Test URL = [**http://localhost:5000/**](http://localhost:5000/)

### Environment variables to run the Project

| Name                    | Type    |
|-------------------------|---------|
| MY_VAR                  | string  |
| HOST                    | string  |
| USER                    | string  |
| DATABASE                | string  |
| PASSWORD                | string  |
| TOKEN_EXPIRES_IN         | string  |
| JWT_SECRET              | string  |
| ACTIVATION_SECRET       | string  |
| JWT_EXPIRES_IN          | string  |
| SMPT_SERVICE            | string  |
| SMPT_HOST               | string  |
| SMPT_PORT               | string  |
| SMPT_PASSWORD           | string  |
| SMPT_MAIL               | string  |
| NODE_DOCKER_PORT        | string  |
| FRONTEND                | string  |
| BUCKET                  | string  |
| PROJECTID               | string  |
| SABRE_USER              | string  |
| SABRE_PASSWORD          | string  |
| SABRE_PCC               | string  |
| SABRE_BASE_CERT_URL     | string  |
| SABRE_BASE_PROD_URL     | string  |
| ADDRESS_LINE            | string  |
| CITY_NAME               | string  |
| COUNTRY_CODE            | string  |
| POSTAL_CODE             | string  |
| STATE_CODE              | string  |
| STREET_NUMBER           | string  |




## Error Handling

Describe the API's error response format and provide common error codes and their meanings.

```javascript
res.status(error.statusCode || 500)
    .json({ success: false, error: error.message || "Server Error", });

````

all errors are handled globally until, and unless when work with third party API like sabre issue with error handling 
 cos, I've less control on those API errors

## Versioning

Currently working on version one i.e /api/v1.

<seealso>

<!--List any additional resources, such as tutorials or guides, that can help users understand and use the API effectively.-->

</seealso>
