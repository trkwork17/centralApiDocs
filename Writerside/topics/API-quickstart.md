# API Quickstart

<!-- This document describes how to start using your API: authorization, authentication, accessing API resources. -->
In this section, you'll find a step-by-step guide to quickly start using the API.

## Prerequisites


* To use the API, you need the API KEY for generate access token if you don't have an API key, please contact us.
* When you have an API key, you have to generate an access token for each request


## Making Your First Request

Provide a simple example of making a request to one of the APIs endpoints. Clear and concise code snippets.

```http
POST /api/v1/api_agent/booking/booking_price HTTP/1.1
Host: https://quickticketsb2b-nodejs.de.r.appspot.com
Authorization: Bearer YOUR_ACCESS_TOKEN
```
 * Request Body
```json
  {
  "adultCount": 1,
  "childCount": 0,
  "infantCount": 0,
  "system": "system001",
  "segment": 1,
  "tripType": "1",
  "segments": [
    {
      "marketingCarrier": "BG",

      "marketingFlightNumber": "434",
      "operatingCarrier": "BG",
      "operatingCareerName": "Biman Bangladesh Airlines",
      "operatingFlight": "434",
      "departure": "CXB",
      "departureAirport": "Cox's Bazar Airport",
      "departureLocation": "Cox's Bazar,Bangladesh",
      "departureTime": "09:40",
      "departureDateTime": "2023-12-25T09:40:00",
      "arrival": "DAC",
      "arrivalAirport": "Hazrat Shahjalal Intl Airport",
      "arrivalLocation": "Dhaka,Bangladesh",
      "arrivalTime": "10:45",
      "arrivalDateTime": "2023-12-25T10:45:00",
      "flightDuration": "1H 5Min",
      "bookingClass": "G"

    }
  ]
}
```
## Response Handling
Explain how to handle the API responses, including parsing JSON data and handling errors.

* Response

**Status 200 OK**

```json
   [
  {
    "segmentType": "oneWay",
    "tripType": "oneWay",
    "journeyType": "Inbound",
    "isRefundable": true,
    "commissionType": "sabredomestic",
    "lastTicketDate": "2023-12-06",
    "validatingCarrier": "BG",
    "basePrice": 4825,
    "clientPrice": 5800,
    "agentPrice": 5094,
    "currency": "BDT",
    "totalTax": 975,
    "ait": 0.003,
    "depCity": "Chittagong",
    "arrCity": "Dhaka",
    "commission": 15,
    "fares": [
      {
        "paxType": "ADT",
        "passengerCount": 1,
        "isRefundable": true,
        "baseFare": 4825,
        "tax": 975,
        "totalTax": 975,
        "totalBaseFareAmount": 4825,
        "totalBaseFareAmountWithTax": 5800,
        "currency": "BDT",
        "clientPrice": 5800,
        "totalClientPrice": 5800,
        "serviceFee": 0,
        "discount": 0,
        "bag": "20 KG"
      }
    ],
    "travelTime": "2023-12-25T09:40:00"
  }
]
```



## API Usage Tips
To use the APIs effectively and efficiently must require basic knowledge of using postman and REST API.

## Next Steps
You can explore more endpoints or integrate the APIs in your applications.