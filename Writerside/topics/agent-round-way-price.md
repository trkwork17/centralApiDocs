# Air Price round Way

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/api_agent/booking/air-price-roundWay" method="post">
    <request>
       <sample lang="JSON">
            {
    "adultCount": 1,
    "childCount": 1,
    "infantCount": 1,
    "tripType": 2,
    "system": "system001",
    "segments": {
        "go": [
            {
                "marketingCarrier": "AA",
                "marketingFlightNumber": 4743,
                "operatingCarrier": "AA",
                "operatingFlightNumber": 4743,
                "departure": "JFK",
                "departureDateTime": "2024-03-23T19:29:00",
                "arrival": "BOS",
                "arrivalDateTime": "2024-03-23T20:48:00",
                "bookingClass": "O"
            },
            {
                "marketingCarrier": "AA",
                "marketingFlightNumber": 8134,
                "operatingCarrier": "QR",
                "operatingFlightNumber": 744,
                "departure": "BOS",
                "departureDateTime": "2024-03-23T22:10:00",
                "arrival": "DOH",
                "arrivalDateTime": "2024-03-24T17:15:00",
                "bookingClass": "O"
            },
            {
                "marketingCarrier": "AA",
                "marketingFlightNumber": 8215,
                "operatingCarrier": "QR",
                "operatingFlightNumber": 642,
                "departure": "DOH",
                "departureDateTime": "2024-03-24T19:25:00",
                "arrival": "DAC",
                "arrivalDate": "2024-03-24",
                "arrivalDateTime": "2024-03-24T03:20:00",
                "bookingClass": "O"
            }
        ],
        "back": [
            {
                "marketingCarrier": "AA",
                "marketingFlightNumber": 8169,
                "operatingCarrier": "QR",
                "operatingFlightNumber": 641,
                "departure": "DAC",
                 "departureDateTime": "2024-04-02T10:55:00",
                "departureCityCode": "DAC",
                "arrival": "DOH",
                "arrivalDateTime": "2024-04-02T13:45:00",
                "bookingClass": "Q"
            },
            {
                "marketingCarrier": "AA",
                "marketingFlightNumber": 8308,
                "operatingCarrier": "QR",
                "operatingFlightNumber": 703,
                "departure": "DOH",
                "departureDateTime": "2024-04-03T01:45:00",
                "arrival": "JFK",
                "arrivalDateTime": "2024-04-03T09:00:00",
                "bookingClass": "Q"
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
    "success": true,
    "message": "successfully get air price",
    "data": [
        {
            "segmentType": "roundWay",
            "tripType": "roundWay",
            "journeyType": "Outbound",
            "isRefundable": false,
            "immediateIssues": 0,
            "commissionType": "sotti",
            "lastTicketDate": "2024-03-03",
            "validatingCarrier": "AA",
            "basePrice": 108240,
            "clientPrice": 267199,
            "agentPrice": 267199,
            "currency": "BDT",
            "totalTax": 158959,
            "depCity": "New York",
            "arrCity": "Dhaka",
            "commission": -10,
            "fares": [
                {
                    "paxType": "ADT",
                    "passengerCount": 1,
                    "isRefundable": false,
                    "baseFare": 56980,
                    "tax": 75985,
                    "totalTax": 75985,
                    "totalBaseFareAmount": 56980,
                    "totalBaseFareAmountWithTax": 132965,
                    "currency": "BDT",
                    "clientPrice": 132965,
                    "totalClientPrice": 132965,
                    "serviceFee": 0,
                    "discount": 0,
                    "agentPrice": 132965,
                    "bag": "1 Piece"
                },
                {
                    "paxType": "CNN",
                    "passengerCount": 1,
                    "isRefundable": false,
                    "baseFare": 42680,
                    "tax": 72985,
                    "totalTax": 72985,
                    "totalBaseFareAmount": 42680,
                    "totalBaseFareAmountWithTax": 115665,
                    "currency": "BDT",
                    "clientPrice": 115665,
                    "totalClientPrice": 115665,
                    "serviceFee": 0,
                    "discount": 0,
                    "agentPrice": 115665,
                    "bag": "1 Piece"
                },
                {
                    "paxType": "INF",
                    "passengerCount": 1,
                    "isRefundable": false,
                    "baseFare": 8580,
                    "tax": 9989,
                    "totalTax": 9989,
                    "totalBaseFareAmount": 8580,
                    "totalBaseFareAmountWithTax": 18569,
                    "currency": "BDT",
                    "clientPrice": 18569,
                    "totalClientPrice": 18569,
                    "serviceFee": 0,
                    "discount": 0,
                    "agentPrice": 18569,
                    "bag": "1 Piece"
                }
            ],
            "travelTime": "2024-03-23T19:29:00"
        }
    ]
}
]
      </sample>  
    </response>
     <response type="401">
        <sample lang="JSON">
            {
  "success": false,
  "message": "No authorization token was found"
}   
      </sample>      
    </response>
  <response type="404">
         <sample lang="JSON">
           {
  "success": false,
  "message": "No fights found"
}
      </sample>   
    </response>
</api-endpoint>