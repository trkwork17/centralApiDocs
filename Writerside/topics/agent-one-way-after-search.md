# one Way After Search


<api-endpoint openapi-path="./../openapi.yaml" endpoint="/api_agent/booking/search-results" method="get">
<request>
        <sample lang="JSON">
         {
  "type": "oneway",
  "adultCount": 1,
  "childCount": 0,
  "infantCount": 0,
  "departure": "DAC",
  "arrival": "CXB",
  "departureDate": "2024-03-10",
  "cabin": "Economy",
  "vendorPref":[],
   "maxStopsQuantity": 1
}
      </sample>      
    </request> 
  <response type="200">
         <sample lang="JSON">
       "results": [
        {
            "uuid": "5939888ff3e9473181fe4fdaafef80bf",
            "system": "system001",
            "tripType": "oneWay",
            "journeyType": "Inbound",
            "segment": 1,
            "lastTicketedTime": "2024-03-01 10:22",
            "basePrice": 5024,
            "agentPrice": 5263,
            "clientPrice": 5999,
            "commission": 736,
            "commissionType": "domestic",
            "commissionValue": 15,
            "class": "Economy",
            "carrierName": "Biman Bangladesh Airlines",
            "taxes": 975,
            "isRefundable": "Refundable",
            "departure": "DAC",
            "arrival": "CXB",
            "carrier": "BG",
            "departureDate": "2024-03-10",
            "departureTime": "12:00:00",
            "arrivalDate": "2024-03-10",
            "arrivalTime": "13:15:00",
            "totalFlightDuration": "1H 15Min",
            "transit": [
                {
                    "transit": "0"
                }
            ],
            "aitPrice": 17.997,
            "baggage": [
                {
                    "id": 1,
                    "paxType": "ADT",
                    "paxCount": 1,
                    "airlineCode": "BG",
                    "weight": 20,
                    "pieceCount": null,
                    "unit": "kg",
                    "allowanceRef": 1
                }
            ],
            "priceBreakdown": [
                {
                    "aitValue": 0.003,
                    "paxType": "ADT",
                    "paxCount": 1,
                    "baseFare": 5024,
                    "tax": 975,
                    "totalTaxAmount": 975,
                    "totalBaseFare": 5024,
                    "totalAmount": 5999,
                    "discount": 0,
                    "otherCharges": 0,
                    "serviceFee": 0
                }
            ],
            "segments": [
                {
                    "departureDateAdjustment": 0,
                    "airCraft": "",
                    "codeShared": "",
                    "marketingCarrier": "BG",
                    "marketingCarrierName": "Biman Bangladesh Airlines",
                    "marketingFlight": 435,
                    "operatingCarrier": "BG",
                    "operatingCarrierName": "Biman Bangladesh Airlines",
                    "operatingFlight": 435,
                    "departure": "DAC",
                    "departureAirport": "Hazrat Shahjalal Intl Airport",
                    "departureCityCode": "DAC",
                    "departureCityName": "Dhaka",
                    "departureCountryCode": "BD",
                    "departureCountryName": "Bangladesh",
                    "departureDateTime": "2024-03-10T12:00:00",
                    "departureTime": "12:00:00",
                    "departureDate": "2024-03-10",
                    "departureLocation": "Dhaka,Bangladesh",
                    "arrival": "CXB",
                    "arrivalAirport": "COX's Bazar Airport",
                    "arrivalCityCode": "CXB",
                    "arrivalCityName": "Cox's Bazar",
                    "arrivalCountryCode": "BD",
                    "arrivalCountryName": "Bangladesh",
                    "arrivalDateTime": "2024-03-10T13:15:00",
                    "arrivalDate": "2024-03-10",
                    "arrivalTime": "13:15:00",
                    "arrivalLocation": "Cox's Bazar,Bangladesh",
                    "flightDuration": "1H 15Min",
                    "bookingClass": "G",
                    "cabinCode": "Y",
                    "mealCode": "S",
                    "Aterminal": "",
                    "Dterminal": "D",
                    "availableSeats": 9,
                    "hiddenStops": []
                }
            ]
        },
      ],
   "searchId": "019504fce9e94f71b7a1ec525709070b"
      </sample>    
    </response>
 <response type="400">
         <sample lang="JSON">
           {
 {
    "success": false,
    "message": "Json Web Token is invalid, Try again"
}
      </sample>   
    </response>
<response type="404">
        <sample lang="JSON">
         []
      </sample>      
    </response>

</api-endpoint>