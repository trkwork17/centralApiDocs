# Air Price multiCity

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/api_agent/booking/air-price" method="post">
    <request>
        <sample lang="JSON">
           {
    "adultCount": 1,
    "childCount": 1,
    "infantCount": 1,
    "system": "system001",
    "tripType": "3",
    "segments": [
        {
            "marketingCarrier": "BS",
            "marketingFlightNumber": 308,
            "operatingCarrier": "BS",
            "operatingFlightNumber": 308,
            "departure": "SIN",
            "departureDateTime": "2024-04-25T05:40:00",
            "arrival": "DAC",
            "arrivalDateTime": "2024-04-25T07:50:00",
            "bookingClass": "S"
        },
        {
            "marketingCarrier": "BS",
            "marketingFlightNumber": 217,
            "operatingCarrier": "BS",
            "operatingFlightNumber": 217,
            "departure": "DAC",
            "departureDateTime": "2024-04-25T10:10:00",
            "arrival": "BKK",
            "arrivalDateTime": "2024-04-25T13:40:00",
            "bookingClass": "S"
        }
    ]
}
      </sample>      
    </request>
    <response type="200">
         <sample lang="JSON">
          [
   {
            "segmentType": "multiCity",
            "tripType": "multiCity",
            "journeyType": "Outbound",
            "isRefundable": true,
            "immediateIssues": 0,
            "commissionType": "sotto",
            "lastTicketDate": "2024-03-04",
            "validatingCarrier": "BS",
            "basePrice": 61340,
            "clientPrice": 72470,
            "agentPrice": 68394,
            "currency": "BDT",
            "totalTax": 11130,
            "depCity": "Singapore",
            "arrCity": "Bangkok",
            "commission": 7,
            "fares": [
                {
                    "paxType": "ADT",
                    "passengerCount": 1,
                    "isRefundable": true,
                    "baseFare": 33123,
                    "tax": 5488,
                    "totalTax": 5488,
                    "totalBaseFareAmount": 33123,
                    "totalBaseFareAmountWithTax": 38611,
                    "currency": "BDT",
                    "clientPrice": 38611,
                    "totalClientPrice": 38611,
                    "serviceFee": 0,
                    "discount": 0,
                    "agentPrice": 36408,
                    "bag": "30 KG"
                },
                {
                    "paxType": "CNN",
                    "passengerCount": 1,
                    "isRefundable": true,
                    "baseFare": 24863,
                    "tax": 5488,
                    "totalTax": 5488,
                    "totalBaseFareAmount": 24863,
                    "totalBaseFareAmountWithTax": 30351,
                    "currency": "BDT",
                    "clientPrice": 30351,
                    "totalClientPrice": 30351,
                    "serviceFee": 0,
                    "discount": 0,
                    "agentPrice": 28702,
                    "bag": "30 KG"
                },
                {
                    "paxType": "INF",
                    "passengerCount": 1,
                    "isRefundable": true,
                    "baseFare": 3354,
                    "tax": 154,
                    "totalTax": 154,
                    "totalBaseFareAmount": 3354,
                    "totalBaseFareAmountWithTax": 3508,
                    "currency": "BDT",
                    "clientPrice": 3508,
                    "totalClientPrice": 3508,
                    "serviceFee": 0,
                    "discount": 0,
                    "agentPrice": 3284,
                    "bag": "10 KG"
                }
            ],
            "travelTime": "2024-04-25T05:40:00"
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