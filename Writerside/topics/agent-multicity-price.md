# Air Price multiCity

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/api_agent/booking/air-price" method="post">
    <request>
        <sample lang="JSON">
           {
    "adultCount": 1,
    "childCount": 0,
    "infantCount": 0,
    "system": "system001",
    "segment": 1,
    "tripType": "3",
    "segments": [
        {
            "marketingCarrier": "SV",
            "marketingFlightNumber": 803,
            "operatingCarrier": "SV",
            "operatingFlightNumber": 803,
            "departure": "DAC",
            "departureDateTime": "2023-12-01T01:50:00",
            "arrival": "JED",
            "arrivalAirPort": "Dubai Intl Airport",
            "arrivalDateTime": "2023-12-01T06:30:00",
            "bookingClass": "T"
        },
        {
            "marketingCarrier": "SV",
            "marketingFlightNumber": 1420,
            "operatingCarrier": "UA",
            "operatingFlightNumber": 1420,
            "departure": "JED",
            "departureDateTime": "2023-12-03T02:10:00",
            "arrival": "MED",
            "arrivalDateTime": "2023-12-03T03:20:00",
            "bookingClass": "T"
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
        "commissionType": "sabresitti",
        "validatingCarrier": "SV",
        "basePrice": 179121,
        "clientPrice": 189673,
        "agentPrice": 176271,
        "currency": "BDT",
        "totalTax": 10552,
        "ait": 0.003,
        "depCity": "Dhaka",
        "arrCity": "Madinah",
        "commission": 7.8,
        "fares": [
            {
                "paxType": "ADT",
                "passengerCount": 1,
                "baseFare": 179121,
                "tax": 10552,
                "totalTax": 10552,
                "totalBaseFareAmount": 179121,
                "totalBaseFareAmountWithTax": 189673,
                "currency": "BDT",
                "clientPrice": 189673,
                "totalClientPrice": 189673,
                "serviceFee": 0,
                "discount": 0,
                "bag": "1 Piece"
            }
        ],
        "travelTime": "2023-12-01T01:50:00"
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