# API Overview

<!-- This document provides an introduction into your API. -->

## Introduction

The Central API seamlessly integrates with Sabre, providing users with powerful features for booking flights,
checking prices, managing bookings, and retrieving information. Users can easily search for one-way, round-trip, or
multi-city flights and get real-time pricing. They can also make hold seats, cancel bookings, and
access detailed booking information. This frontend-friendly solution optimizes the user experience for all
flight-related tasks, enhancing travel planning.

## What you can do using <API name>

1. **Create Air Search Request:**

- Perform air search requests for one-way, round-way, and multi-city flights.

2. **Air Price Retrieve:**

- Before booking, retrieve the latest price information for specific flight services.

3. **Hold a Flight:**

- Book any flight according to your travel needs.

4. **Air Retrieve:**

- After booking, retrieve information such as cancel time limit and other travel-related details.

5. **Provide Passenger Information:**

- To confirm the booking request, provide all necessary parameters for your passengers.

> (**terms and conditions apply**)
>
{style="note"}

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

The current development focuses on version one (/api/v1) of the Central API. Additionally, version two is on the
horizon, bringing further enhancements and features to the platform. Stay tuned for updates and exciting developments as
v2 approaches.

<seealso>

<!--List any additional resources, such as tutorials or guides, that can help users understand and use the API effectively.-->

</seealso>
