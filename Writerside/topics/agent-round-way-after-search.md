# round Way After Search

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/api_agent/booking/search-resultsRound" method="get">
  <response type="200">
         <sample lang="JSON">
         {
        "uId": "b3b332c8636e4048884c2730cd000fc8",
        "system": "sabre",
        "segment": 2,
        "tripType": "OutBound",
        "carrier": "KU",
        "carrierName": "Kuwait Airways",
        "lastTicketedTime": "2023-12-20 17:00",
        "basePrice": 2941952,
        "taxes": 145796,
        "agentPrice": 2861655.0840000003,
        "clientPrice": 3087748,
        "commission": 226093,
        "commissionType": "sotti",
        "commissionValue": 8,
        "fareCurrency": "BDT",
        "baggage": "2 Piece",
        "class": "Business",
        "availableSeat": "9",
        "priceBreakdown": [
            {
                "paxType": "ADT",
                "paxCount": 4,
                "baseFare": 735488,
                "totalBaseFare": 2941952,
                "Tax": 36449,
                "totalTaxAmount": 145796,
                "totalAmount": 3087748,
                "discount": 0,
                "otherCharges": 0,
                "serviceFee": 0
            }
        ],
        "godeparture": "JFK",
        "godepartureTime": "17:00",
        "godepartureDate": "2023-12-20",
        "goarrival": "DAC",
        "goarrivalTime": "01:20",
        "goarrivalDate": "2023-12-22",
        "backdeparture": "DAC",
        "backdepartureTime": "02:40",
        "backdepartureDate": "2024-01-01",
        "backarrival": "JFK",
        "backarrivalTime": "14:25",
        "backarrivalDate": "2024-01-01",
        "totalGoFlightDuration": "16H 50Min",
        "totalBackFlightDuration": "19H 40Min",
        "transit": {
            "go": {
                "Transit 1": "4H 30Min"
            },
            "back": {
                "Transit 1": "3H 5Min"
            }
        },
        "isRefundable": "Refundable",
        "segments": {
            "go": [
                {
                    "aircraft": "BOEING 777-300ER",
                    "marketingCarrier": "KU",
                    "marketingCarrierName": "Kuwait Airways",
                    "marketingFlight": 118,
                    "operatingCarrier": "KU",
                    "operatingCarrierName": "Kuwait Airways",
                    "operatingFlight": 118,
                    "departure": "JFK",
                    "departureAirport": "John F Kennedy Intl ",
                    "departureLocation": "New York,UNITED STATES",
                    "departureCity": "New York",
                    "departureCountryCode": "US",
                    "departureCountryName": "UNITED STATES",
                    "departureTime": "17:00:00",
                    "departureDate": "2023-12-20",
                    "departureDateTime": "2023-12-20T17:00:00",
                    "arrival": "KWI",
                    "arrivalTime": "13:00:00",
                    "arrivalDate": "2023-12-21",
                    "arrivalDateTime": "2023-12-21T13:00:00",
                    "arrivalAirport": "Kuwait Intl Airport",
                    "arrivalLocation": "Kuwait,KUWAIT",
                    "arrivalCity": "Kuwait",
                    "arrivalCountryCode": "KW",
                    "arrivalCountryName": "KUWAIT",
                    "flightDuration": "12H 0Min",
                    "bookingClass": "P",
                    "cabinCode": "C",
                    "mealCode": "M",
                    "baggage": "2 Piece",
                    "availableSeat": "9"
                },
                {
                    "aircraft": "BOEING 777-300ER",
                    "marketingCarrier": "KU",
                    "marketingCarrierName": "Kuwait Airways",
                    "marketingFlight": 283,
                    "operatingCarrier": "KU",
                    "operatingCarrierName": "Kuwait Airways",
                    "operatingFlight": 283,
                    "departure": "KWI",
                    "departureAirport": "Kuwait Intl Airport",
                    "departureLocation": "Kuwait,KUWAIT",
                    "departureCity": "Kuwait",
                    "departureCountryCode": "KW",
                    "departureCountryName": "KUWAIT",
                    "departureTime": "17:30:00",
                    "departureDate": "2023-12-21",
                    "departureDateTime": "2023-12-21T17:30:00",
                    "arrival": "DAC",
                    "arrivalTime": "01:20:00",
                    "arrivalDate": "2023-12-22",
                    "arrivalDateTime": "2023-12-22T01:20:00",
                    "arrivalAirport": "Hazrat Shahjalal Intl Airport",
                    "arrivalLocation": "Dhaka,Bangladesh",
                    "arrivalCity": "Dhaka",
                    "arrivalCountryCode": "BD",
                    "arrivalCountryName": "BANGLADESH",
                    "flightDuration": "4H 50Min",
                    "bookingClass": "P",
                    "cabinCode": "C",
                    "mealCode": "M",
                    "baggage": "2 Piece",
                    "availableSeat": "9"
                }
            ],
            "back": [
                {
                    "aircraft": "BOEING 777-300ER",
                    "marketingCarrier": "KU",
                    "marketingCarrierName": "Kuwait Airways",
                    "marketingFlight": 284,
                    "operatingCarrier": "KU",
                    "operatingCarrierName": "Kuwait Airways",
                    "operatingFlight": 284,
                    "departure": "DAC",
                    "departureAirport": "Hazrat Shahjalal Intl Airport",
                    "departureLocation": "Dhaka,Bangladesh",
                    "departureCity": "Dhaka",
                    "departureCountryCode": "BD",
                    "departureCountryName": "BANGLADESH",
                    "departureTime": "02:40:00",
                    "departureDate": "2024-01-01",
                    "departureDateTime": "2024-01-01T02:40:00",
                    "arrival": "KWI",
                    "arrivalTime": "06:00:00",
                    "arrivalDate": "2024-01-01",
                    "arrivalDateTime": "2024-01-01T06:00:00",
                    "arrivalAirport": "Kuwait Intl Airport",
                    "arrivalLocation": "Kuwait,KUWAIT",
                    "arrivalCity": "Kuwait",
                    "arrivalCountryCode": "KW",
                    "arrivalCountryName": "KUWAIT",
                    "flightDuration": "6H 20Min",
                    "bookingClass": "P",
                    "cabinCode": "C",
                    "mealCode": "M",
                    "baggage": "2 Piece",
                    "availableSeat": "9"
                },
                {
                    "aircraft": "",
                    "marketingCarrier": "KU",
                    "marketingCarrierName": "Kuwait Airways",
                    "marketingFlight": 117,
                    "operatingCarrier": "KU",
                    "operatingCarrierName": "Kuwait Airways",
                    "operatingFlight": 117,
                    "departure": "KWI",
                    "departureAirport": "Kuwait Intl Airport",
                    "departureLocation": "Kuwait,KUWAIT",
                    "departureCity": "Kuwait",
                    "departureCountryCode": "KW",
                    "departureCountryName": "KUWAIT",
                    "departureTime": "09:05:00",
                    "departureDate": "2024-01-01",
                    "departureDateTime": "2024-01-01T09:05:00",
                    "arrival": "JFK",
                    "arrivalTime": "14:25:00",
                    "arrivalDate": "2024-01-01",
                    "arrivalDateTime": "2024-01-01T14:25:00",
                    "arrivalAirport": "John F Kennedy Intl ",
                    "arrivalLocation": "New York,UNITED STATES",
                    "arrivalCity": "New York",
                    "arrivalCountryCode": "US",
                    "arrivalCountryName": "UNITED STATES",
                    "flightDuration": "13H 20Min",
                    "bookingClass": "P",
                    "cabinCode": "C",
                    "mealCode": "M",
                    "baggage": "2 Piece",
                    "availableSeat": "9"
                }
            ]
        }
    }
      </sample>    
    </response>
 <response type="400">
         <sample lang="JSON">
           {
 {
    "success": false,
    "error": "Json Web Token is invalid, Try again"
}
      </sample>   
    </response>
<response type="404">
        <sample lang="JSON">
         []
      </sample>      
    </response>

</api-endpoint>