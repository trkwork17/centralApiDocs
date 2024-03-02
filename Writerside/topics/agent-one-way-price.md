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
    "tripType": 1,
    "segments": [
        {     "marketingCarrier": "QR",
            "marketingFlightNumber": 643,
            "operatingCarrier": "QR",
            "operatingFlightNumber": 643,
            "departure": "DAC",
            "departureDateTime": "2024-03-20T05:20:00",
            "arrival": "DOH",
            "arrivalDateTime": "2024-03-20T08:35:00",
            "bookingClass": "O"
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
            "immediateIssues": 0,
            "commissionType": "sitti",
            "validatingCarrier": "QR",
            "basePrice": 186120,
            "clientPrice": 205312,
            "agentPrice": 185082,
            "currency": "BDT",
            "totalTax": 19192,
            "depCity": "Dhaka",
            "arrCity": "Doha",
            "commission": 11.2,
            "fares": [
                {
                    "paxType": "ADT",
                    "passengerCount": 1,
                    "isRefundable": true,
                    "baseFare": 97900,
                    "tax": 9331,
                    "totalTax": 9331,
                    "totalBaseFareAmount": 97900,
                    "totalBaseFareAmountWithTax": 107231,
                    "currency": "BDT",
                    "clientPrice": 107231,
                    "totalClientPrice": 107231,
                    "serviceFee": 0,
                    "discount": 0,
                    "agentPrice": 96588,
                    "bag": "30 KG"
                },
                {
                    "paxType": "CNN",
                    "passengerCount": 1,
                    "isRefundable": true,
                    "baseFare": 73480,
                    "tax": 7331,
                    "totalTax": 7331,
                    "totalBaseFareAmount": 73480,
                    "totalBaseFareAmountWithTax": 80811,
                    "currency": "BDT",
                    "clientPrice": 80811,
                    "totalClientPrice": 80811,
                    "serviceFee": 0,
                    "discount": 0,
                    "agentPrice": 72824,
                    "bag": "30 KG"
                },
                {
                    "paxType": "INF",
                    "passengerCount": 1,
                    "isRefundable": true,
                    "baseFare": 14740,
                    "tax": 2530,
                    "totalTax": 2530,
                    "totalBaseFareAmount": 14740,
                    "totalBaseFareAmountWithTax": 17270,
                    "currency": "BDT",
                    "clientPrice": 17270,
                    "totalClientPrice": 17270,
                    "serviceFee": 0,
                    "discount": 0,
                    "agentPrice": 15671,
                    "bag": "10 KG"
                }
            ],
            "travelTime": "2024-03-20T05:20:00",
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