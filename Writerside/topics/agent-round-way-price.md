# Air Price round Way

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/api_agent/booking/air-price-roundWay" method="post">
    <request>
       <sample lang="JSON">
             {
  "adultCount": 1,
  "childCount": 0,
  "infantCount": 0,
  "tripType": 2,
  "system": "system001",
  "segments": {
    "go": [
      {
        "marketingCareer": "EK",
        "marketingFlight": 587,
        "operatingCareer": "QR",
        "operatingFlight": 587,
        "departure": "DAC",
        "departureDateTime": "2024-01-04T18:40:00",
        "arrival": "DXB",
        "arrivalDateTime": "2024-01-04T22:10:00",
        "bookingCode": "M"
      },
      {
        "marketingCareer": "EK",
        "marketingFlight": 203,
        "operatingCareer": "EK",
        "operatingFlight": 203,
        "departure": "DXB",
        "departureDateTime": "2024-01-05T02:35:00",
        "arrival": "JFK",
        "arrivalDateTime": "2024-01-05T08:15:00",
        "bookingCode": "M"
      }
    ],
    "back": [
      {
        "marketingCareer": "EK",
        "marketingFlight": 204,
        "operatingCareer": "EK",
        "operatingFlight": 204,
        "departure": "JFK",
        "departureDateTime": "2024-01-10T10:40:00",
        "arrival": "DXB",
        "arrivalDateTime": "2024-01-11T08:10:00",
        "bookingCode": "L"
      },
      {
        "marketingCareer": "EK",
        "marketingFlight": 584,
        "operatingCareer": "EK",
        "operatingFlight": 584,
        "departure": "DXB",
        "departureDateTime": "2024-01-11T16:45:00",
        "arrival": "DAC",
        "arrivalDateTime": "2024-01-11T23:00:00",
        "bookingCode": "L"
      }
    ]
  }
}
       </sample>
    </request>
    <response type="200">
       <sample lang="JSON">
        [
  {
    "segmentType": "roundWay",
    "tripType": "roundWay",
    "journeyType": "Outbound",
    "isRefundable": true,
    "commissionType": "sabresotti",
    "lastTicketDate": "2023-11-30",
    "validatingCarrier": "BS",
    "basePrice": 18958,
    "clientPrice": 22571,
    "agentPrice": 20345,
    "currency": "BDT",
    "totalTax": 3613,
    "ait": 0.003,
    "depCity": "Dubai",
    "arrCity": "Dhaka",
    "commission": 12.1,
    "fares": [
      {
        "paxType": "ADT",
        "passengerCount": 1,
        "baseFare": 18958,
        "tax": 3613,
        "totalTax": 3613,
        "totalBaseFareAmount": 18958,
        "totalBaseFareAmountWithTax": 22571,
        "currency": "BDT",
        "clientPrice": 22571,
        "totalClientPrice": 22571,
        "serviceFee": 0,
        "discount": 0,
        "bag": "0 KG"
      }
    ],
    "travelTime": "2023-12-20T21:45:00"
  }
]
      </sample>  
    </response>
     <response type="401">
        <sample lang="JSON">
            {
  "success": false,
  "error": "No authorization token was found"
}   
      </sample>      
    </response>
  <response type="404">
         <sample lang="JSON">
           {
  "success": false,
  "error": "No fights found"
}
      </sample>   
    </response>
</api-endpoint>