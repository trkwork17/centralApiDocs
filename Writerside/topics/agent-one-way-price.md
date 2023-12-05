# Air Price one Way

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/api_agent/booking/air-price" method="post">
    <request>
        <sample>
          {
  "adultCount": 1,
  "childCount": 0,
  "infantCount": 0,
  "system": "system001",
  "segment": 1,
  "tripType": "1",
  "segments": [
    {
      "marketingCareer": "BS",
      "marketingFlight": "342",
      "operatingCareer": "BS",
      "operatingFlight": "342",
      "departure": "DXB",
      "departureDateTime": "2023-12-20T21:45:00",
      "arrival": "DAC",
      "arrivalDateTime": "2023-12-20T04:20:00",
      "bookingCode": "S"
    }
  ]
}
       </sample>
    </request>
    <response type="200">
         <sample lang="JSON">
        [
  {
    "segmentType": "oneWay",
    "tripType": "oneWay",
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