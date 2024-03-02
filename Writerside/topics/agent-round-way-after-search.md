# round Way After Search 

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/api_agent/booking/search-resultsRound" method="get">
 <request>
        <sample lang="JSON">
        {
    "type": "roundway",
    "departureDate": "2024-03-23",
    "departure": "JFK",
    "arrival": "DAC",
    "arrivalDate": "2024-04-02",
    "adultCount": 1,
    "childCount": 0,
    "infantCount": 0,
    "cabin": "Economy",
    "vendorPref":[],
    "maxStopsQuantity": 0
}
      </sample>      
    </request> 
  <response type="200">
         <sample lang="JSON">
         "results": [
       {
            "uuid": "7ab009a033ab47969c86ef50683768d0",
            "system": "system001",
            "tripType": "roundway",
            "goSegment": 3,
            "backSegment": 2,
            "journeyType": "Outbound",
            "lastTicketedTime": "2024-03-03 23:59",
            "basePrice": 48510,
            "agentPrice": 120017,
            "clientPrice": 124495,
            "commission": 4478,
            "commissionType": "sotti",
            "commissionValue": 10,
            "isRefundable": "NonRefundable",
            "carrier": "AA",
            "carrierName": "American Airlines",
            "baggage": {
                "go": [
                    {
                        "id": 5,
                        "paxType": "ADT",
                        "paxCount": 1,
                        "airlineCode": "AA",
                        "weight": null,
                        "pieceCount": 1,
                        "unit": null,
                        "allowanceRef": 5
                    }
                ],
                "back": [
                    {
                        "id": 5,
                        "paxType": "ADT",
                        "paxCount": 1,
                        "airlineCode": "AA",
                        "weight": null,
                        "pieceCount": 1,
                        "unit": null,
                        "allowanceRef": 5
                    }
                ]
            },
            "tax": 75985,
            "totalFlightDurationGo": "21H 51Min",
            "totalFlightDurationBack": "32H 5Min",
            "class": "Economy",
            "goDepartureDate": "2024-03-23",
            "goDepartureTime": "19:29:00",
            "goArrivalTime": "03:20:00",
            "goArrivalDate": "2024-03-24",
            "goDeparture": "JFK",
            "goArrival": "DAC",
            "backDepartureDate": "2024-04-02",
            "backDepartureTime": "10:55:00",
            "backArrivalDate": "2024-04-03",
            "backDeparture": "DAC",
            "backArrival": "JFK",
            "aitPrice": 373.485,
            "backArrivalTime": "09:00:00",
            "transit": {
                "go": [
                    {
                        "transit": "1H 22Min"
                    },
                    {
                        "transit": "2H 10Min"
                    }
                ],
                "back": [
                    {
                        "transit": "12H 0Min"
                    }
                ]
            },
            "priceBreakdown": [
                {
                    "aitValue": 0.003,
                    "paxType": "ADT",
                    "paxCount": 1,
                    "baseFare": 48510,
                    "tax": 75985,
                    "totalBaseFare": 48510,
                    "totalTaxAmount": 75985,
                    "totalAmount": 124495,
                    "discount": 0,
                    "otherCharges": 0,
                    "serviceFee": 0
                }
            ],
            "segments": {
                "go": [
                    {
                        "departureDateAdjustment": 0,
                        "codeShared": "REPUBLIC AIRWAYS AS AMERICAN EAGLE",
                        "totalElapsedTime": 1311,
                        "airCraft": "EMBRAER EMB 175",
                        "marketingCarrier": "AA",
                        "marketingCarrierName": "American Airlines",
                        "marketingFlight": 4743,
                        "operatingCarrier": "AA",
                        "operatingCarrierName": "American Airlines",
                        "operatingFlight": 4743,
                        "departure": "JFK",
                        "departureAirport": "John F Kennedy Intl ",
                        "departureCityCode": "NYC",
                        "departureCityName": "New York",
                        "departureCountryCode": "US",
                        "departureDateTime": "2024-03-23T19:29:00",
                        "departureCountryName": "United States",
                        "departureTime": "19:29:00",
                        "departureDate": "2024-03-23",
                        "departureLocation": "New York,United States",
                        "arrival": "BOS",
                        "arrivalAirport": "Logan Intl Airport",
                        "arrivalCityCode": "BOS",
                        "arrivalCityName": "Boston",
                        "arrivalCountryCode": "US",
                        "arrivalCountryName": "United States",
                        "arrivalLocation": "Boston,United States",
                        "arrivalTime": "20:48:00",
                        "arrivalDate": "2024-03-23",
                        "arrivalDateTime": "2024-03-23T20:48:00",
                        "flightDuration": "1H 19Min",
                        "dateAdjustment": 0,
                        "Aterminal": "B",
                        "Dterminal": "8",
                        "goSegmentCode": {
                            "bookingClass": "O",
                            "cabinCode": "Y",
                            "mealCode": "",
                            "availableSeats": 7
                        },
                        "hiddenStops": []
                    },
                    {
                        "departureDateAdjustment": 0,
                        "codeShared": "",
                        "totalElapsedTime": 1311,
                        "airCraft": "AIRBUS A359",
                        "marketingCarrier": "AA",
                        "marketingCarrierName": "American Airlines",
                        "marketingFlight": 8134,
                        "operatingCarrier": "QR",
                        "operatingCarrierName": "Qatar Airways",
                        "operatingFlight": 744,
                        "departure": "BOS",
                        "departureAirport": "Logan Intl Airport",
                        "departureCityCode": "BOS",
                        "departureCityName": "Boston",
                        "departureCountryCode": "US",
                        "departureDateTime": "2024-03-23T22:10:00",
                        "departureCountryName": "United States",
                        "departureTime": "22:10:00",
                        "departureDate": "2024-03-23",
                        "departureLocation": "Boston,United States",
                        "arrival": "DOH",
                        "arrivalAirport": "Doha Hamad INTL Airport",
                        "arrivalCityCode": "DOH",
                        "arrivalCityName": "Doha",
                        "arrivalCountryCode": "QA",
                        "arrivalCountryName": "Qatar",
                        "arrivalLocation": "Doha,Qatar",
                        "arrivalTime": "17:15:00",
                        "arrivalDate": "2024-03-24",
                        "arrivalDateTime": "2024-03-24T17:15:00",
                        "flightDuration": "12H 5Min",
                        "dateAdjustment": 1,
                        "Aterminal": "",
                        "Dterminal": "E",
                        "goSegmentCode": {
                            "bookingClass": "O",
                            "cabinCode": "Y",
                            "mealCode": "M",
                            "availableSeats": 7
                        },
                        "hiddenStops": []
                    },
                    {
                        "departureDateAdjustment": 1,
                        "codeShared": "",
                        "totalElapsedTime": 1311,
                        "airCraft": "AIRBUS INDUSTRIE 330-300",
                        "marketingCarrier": "AA",
                        "marketingCarrierName": "American Airlines",
                        "marketingFlight": 8215,
                        "operatingCarrier": "QR",
                        "operatingCarrierName": "Qatar Airways",
                        "operatingFlight": 642,
                        "departure": "DOH",
                        "departureAirport": "Doha Hamad INTL Airport",
                        "departureCityCode": "DOH",
                        "departureCityName": "Doha",
                        "departureCountryCode": "QA",
                        "departureDateTime": "2024-03-24T19:25:00",
                        "departureCountryName": "Qatar",
                        "departureTime": "19:25:00",
                        "departureDate": "2024-03-24",
                        "departureLocation": "Doha,Qatar",
                        "arrival": "DAC",
                        "arrivalAirport": "Hazrat Shahjalal Intl Airport",
                        "arrivalCityCode": "DAC",
                        "arrivalCityName": "Dhaka",
                        "arrivalCountryCode": "BD",
                        "arrivalCountryName": "Bangladesh",
                        "arrivalLocation": "Dhaka,Bangladesh",
                        "arrivalTime": "03:20:00",
                        "arrivalDate": "2024-03-24",
                        "arrivalDateTime": "2024-03-24T03:20:00",
                        "flightDuration": "4H 55Min",
                        "dateAdjustment": 1,
                        "Aterminal": "1",
                        "Dterminal": "",
                        "goSegmentCode": {
                            "bookingClass": "O",
                            "cabinCode": "Y",
                            "mealCode": "M",
                            "availableSeats": 7
                        },
                        "hiddenStops": []
                    }
                ],
                "back": [
                    {
                        "departureDateAdjustment": 0,
                        "codeShared": "",
                        "totalElapsedTime": 1925,
                        "airCraft": "AIRBUS INDUSTRIE 330-300",
                        "marketingCarrier": "AA",
                        "marketingCarrierName": "American Airlines",
                        "marketingFlight": 8169,
                        "operatingCarrier": "QR",
                        "operatingCarrierName": "Qatar Airways",
                        "operatingFlight": 641,
                        "departure": "DAC",
                        "departureAirport": "Hazrat Shahjalal Intl Airport",
                        "departureCityCode": "DAC",
                        "departureCityName": "Dhaka",
                        "departureCountryCode": "BD",
                        "departureDateTime": "2024-04-02T10:55:00",
                        "departureCountryName": "Bangladesh",
                        "departureTime": "10:55:00",
                        "departureDate": "2024-04-02",
                        "departureLocation": "Dhaka,Bangladesh",
                        "arrival": "DOH",
                        "arrivalAirport": "Doha Hamad INTL Airport",
                        "arrivalCityCode": "DOH",
                        "arrivalCityName": "Doha",
                        "arrivalCountryCode": "QA",
                        "arrivalCountryName": "Qatar",
                        "arrivalLocation": "Doha,Qatar",
                        "arrivalTime": "13:45:00",
                        "arrivalDate": "2024-04-02",
                        "arrivalDateTime": "2024-04-02T13:45:00",
                        "flightDuration": "5H 50Min",
                        "dateAdjustment": 0,
                        "Aterminal": "",
                        "Dterminal": "1",
                        "backSegmentCode": {
                            "bookingClass": "Q",
                            "cabinCode": "Y",
                            "mealCode": "M",
                            "availableSeats": 7
                        },
                        "hiddenStops": []
                    },
                    {
                        "departureDateAdjustment": 1,
                        "codeShared": "",
                        "totalElapsedTime": 1925,
                        "airCraft": "BOEING 777",
                        "marketingCarrier": "AA",
                        "marketingCarrierName": "American Airlines",
                        "marketingFlight": 8308,
                        "operatingCarrier": "QR",
                        "operatingCarrierName": "Qatar Airways",
                        "operatingFlight": 703,
                        "departure": "DOH",
                        "departureAirport": "Doha Hamad INTL Airport",
                        "departureCityCode": "DOH",
                        "departureCityName": "Doha",
                        "departureCountryCode": "QA",
                        "departureDateTime": "2024-04-03T01:45:00",
                        "departureCountryName": "Qatar",
                        "departureTime": "01:45:00",
                        "departureDate": "2024-04-03",
                        "departureLocation": "Doha,Qatar",
                        "arrival": "JFK",
                        "arrivalAirport": "John F Kennedy Intl ",
                        "arrivalCityCode": "NYC",
                        "arrivalCityName": "New York",
                        "arrivalCountryCode": "US",
                        "arrivalCountryName": "United States",
                        "arrivalLocation": "New York,United States",
                        "arrivalTime": "09:00:00",
                        "arrivalDate": "2024-04-03",
                        "arrivalDateTime": "2024-04-03T09:00:00",
                        "flightDuration": "14H 15Min",
                        "dateAdjustment": 0,
                        "Aterminal": "8",
                        "Dterminal": "",
                        "backSegmentCode": {
                            "bookingClass": "Q",
                            "cabinCode": "Y",
                            "mealCode": "M",
                            "availableSeats": 7
                        },
                        "hiddenStops": []
                    }
                ]
            }
        },
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