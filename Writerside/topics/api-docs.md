# API Overview

<!-- This document provides an introduction into your API. -->

## Introduction

The Central API with Node.js and Express.js is a frontend-friendly serverside that handles user operations and
provides optimal routes.

## What you can do using <API name>

1. **Create Air Search Request:**
 - Perform air search requests for one-way, round-way, and multi-city flights.

2. **Air Price Retrieve:**
 - Before booking, retrieve the latest price information for specific flight services.

3. **Book a Flight:**
 - Book any flight according to your travel needs.

4. **Air Retrieve:**
 - After booking, retrieve information such as cancel time limit and other travel-related details.

5. **Provide Passenger Information:**
 - To confirm the booking request, provide all necessary parameters for your passengers.

6. **Cancel, Reissue, Refund, and Void Requests:**
 - During the time limit period, perform operations like cancel, reissue, refund, and void 
>(**terms and conditions apply**)
> 
   {style="note"}

7. **Wallet Deposit:**
 - Deposit any amount of money into your wallet for future purchases.

8. **Wallet Withdrawal:**
 - Withdraw any amount of money from your wallet if needed.

## Authentication
To perform any task on the secure route, you must provide your credentials to the application.
To do this, you need to provide a Bearer token.

1. **Provide Credentials:**
 - Ensure you have valid credentials for authentication.

2. **Include Bearer Token:**
 - To perform any task, include a Bearer token in your requests.




## Base URL

**Live URL** = [**https://quickticketsb2b-nodejs.de.r.appspot.com/**](https://quickticketsb2b-nodejs.de.r.appspot.com/)







## Error Handling

Describe the APIs error response format and provide common error codes and their meanings.

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
