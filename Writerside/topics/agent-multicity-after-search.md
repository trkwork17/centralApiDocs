# multiCity After Search


<api-endpoint openapi-path="./../openapi.yaml" endpoint="/api_agent/booking/search-multiCity" method="get">
<request>
        <sample lang="JSON">
           {
  "type": "multicity",
  "adultCount": 1,
  "childCount": 0,
  "infantCount": 0,
   "cabin":"Business",
  "segmentsList": [
    {
      "departure": "DAC",
      "arrival": "JED",
      "departureDate": "2024-02-03"
    },
    {
      "departure": "DXB",
      "arrival": "MED",
      "departureDate": "2024-02-15"
    },
    {
      "departure": "BKK",
      "arrival": "SIN",
      "departureDate": "2024-03-01"
    }
  ]
}
      </sample>      
    </request> 
<response type="200">
         <sample lang="JSON">
       {
        "uId": "60581b3ddf3449c8af44a2eab0c39926",
        "system": "system001",
        "carrier": "BG",
        "carrierName": "Biman Bangladesh Airlines",
        "segment": 2,
        "baseFare": 487305,
        "class": "Business",
        "taxes": 49674,
        "commissionType": "sitti",
        "agentPrice": 484986,
        "clientPrice": 536979,
        "commission": 51993,
        "commissionValue": 11,
        "availableSeat": "9",
        "priceBreakdown": [
            {
                "paxType": "ADT",
                "paxCount": 1,
                "baseFare": 487305,
                "totalBaseFare": 487305,
                "tax": 49674,
                "totalTaxAmount": 49674,
                "totalAmount": 536979,
                "discount": 0,
                "otherCharges": 0,
                "serviceFee": 0
            }
        ],
        "cityCount": [
            {
                "departureDate": "2024-02-03",
                "departure": "DAC",
                "arrival": "JED",
                "legIndex": 1,
                "flightIndex": 1,
                "segments": [
                    {
                        "aircraft": "BOEING 777-300",
                        "marketingCarrier": "BG",
                        "marketingCarrierName": "Biman Bangladesh Airlines",
                        "marketingFlightNumber": 335,
                        "operatingCarrier": "BG",
                        "operatingFlightNumber": 335,
                        "operatingCarrierName": "Biman Bangladesh Airlines",
                        "departureCity": "Dhaka",
                        "departureCountryCode": "BD",
                        "departureCountryName": "BANGLADESH",
                        "departure": "DAC",
                        "departureAirPort": "Hazrat Shahjalal Intl Airport",
                        "departureLocation": "Dhaka,Bangladesh",
                        "departureDate": "2024-02-03",
                        "departureDateTime": "2024-02-03T16:45:00",
                        "departureTime": "16:45:00",
                        "arrivalCity": "Jeddah",
                        "arrivalCountryCode": "SA",
                        "arrivalCountryName": "SAUDI ARABIA",
                        "arrival": "JED",
                        "arrivalAirPort": "Jeddah Intl ",
                        "arrivalLocation": "Jeddah,SAUDI ARABIA",
                        "arrivalDate": "2024-02-03",
                        "arrivalDateTime": "2024-02-03T21:25:00",
                        "arrivalTime": "21:25:00",
                        "baggage": "40 KG",
                        "bookingClass": "J",
                        "cabinCode": "C",
                        "mealCode": "M",
                        "stopCount": 0,
                        "flightDuration": "7H 40Min"
                    }
                ]
            },
            {
                "departureDate": "2024-02-15",
                "departure": "DXB",
                "arrival": "MED",
                "legIndex": 2,
                "flightIndex": 1,
                "segments": [
                    {
                        "aircraft": "AIRBUS A320NEO",
                        "marketingCarrier": "MS",
                        "marketingCarrierName": "EgyptAir",
                        "marketingFlightNumber": 906,
                        "operatingCarrier": "MS",
                        "operatingFlightNumber": 906,
                        "operatingCarrierName": "EgyptAir",
                        "departureCity": "Dubai",
                        "departureCountryCode": "AE",
                        "departureCountryName": "UNITED ARAB EMIRATES",
                        "departure": "DXB",
                        "departureAirPort": "Dubai Intl Airport",
                        "departureLocation": "Dubai,UNITED ARAB EMIRATES",
                        "departureDate": "2024-02-15",
                        "departureDateTime": "2024-02-15T19:00:00",
                        "departureTime": "19:00:00",
                        "arrivalCity": "Cairo",
                        "arrivalCountryCode": "EG",
                        "arrivalCountryName": "EGYPT",
                        "arrival": "CAI",
                        "arrivalAirPort": "Cairo Intl Airport",
                        "arrivalLocation": "Cairo,EGYPT",
                        "arrivalDate": "2024-02-15",
                        "arrivalDateTime": "2024-02-15T21:00:00",
                        "arrivalTime": "21:00:00",
                        "baggage": "40 KG",
                        "bookingClass": "J",
                        "cabinCode": "C",
                        "mealCode": "M",
                        "stopCount": 0,
                        "flightDuration": "4H 0Min"
                    },
                    {
                        "aircraft": "AIRBUS",
                        "marketingCarrier": "MS",
                        "marketingCarrierName": "EgyptAir",
                        "marketingFlightNumber": 675,
                        "operatingCarrier": "MS",
                        "operatingFlightNumber": 675,
                        "operatingCarrierName": "EgyptAir",
                        "departureCity": "Cairo",
                        "departureCountryCode": "EG",
                        "departureCountryName": "EGYPT",
                        "departure": "CAI",
                        "departureAirPort": "Cairo Intl Airport",
                        "departureLocation": "Cairo,EGYPT",
                        "departureDate": "2024-02-15",
                        "departureDateTime": "2024-02-15T22:40:00",
                        "departureTime": "22:40:00",
                        "arrivalCity": "Madinah",
                        "arrivalCountryCode": "SA",
                        "arrivalCountryName": "SAUDI ARABIA",
                        "arrival": "MED",
                        "arrivalAirPort": "Prince Mohammad Bin Abdulaziz Intl Airport",
                        "arrivalLocation": "Madinah,SAUDI ARABIA",
                        "arrivalDate": "2000-01-02",
                        "arrivalDateTime": "2024-02-16T01:20:00",
                        "arrivalTime": "01:20:00",
                        "baggage": "40 KG",
                        "bookingClass": "J",
                        "cabinCode": "C",
                        "mealCode": "M",
                        "stopCount": 0,
                        "flightDuration": "1H 40Min"
                    }
                ],
                "transit": {
                    "Transit": "1 hours 40 minutes"
                }
            },
            {
                "departureDate": "2024-03-01",
                "departure": "BKK",
                "arrival": "SIN",
                "legIndex": 3,
                "flightIndex": 1,
                "segments": [
                    {
                        "aircraft": "AIRBUS A359",
                        "marketingCarrier": "TG",
                        "marketingCarrierName": "Thai Airways",
                        "marketingFlightNumber": 403,
                        "operatingCarrier": "TG",
                        "operatingFlightNumber": 403,
                        "operatingCarrierName": "Thai Airways",
                        "departureCity": "Bangkok",
                        "departureCountryCode": "TH",
                        "departureCountryName": "THAILAND",
                        "departure": "BKK",
                        "departureAirPort": "Suvarnabhumi Intl Airport",
                        "departureLocation": "Bangkok,THAILAND",
                        "departureDate": "2024-03-01",
                        "departureDateTime": "2024-03-01T08:00:00",
                        "departureTime": "08:00:00",
                        "arrivalCity": "Singapore",
                        "arrivalCountryCode": "SG",
                        "arrivalCountryName": "SINGAPORE",
                        "arrival": "SIN",
                        "arrivalAirPort": "Changi Intl Airport",
                        "arrivalLocation": "Singapore,SINGAPORE",
                        "arrivalDate": "2024-03-01",
                        "arrivalDateTime": "2024-03-01T11:15:00",
                        "arrivalTime": "11:15:00",
                        "baggage": "40 KG",
                        "bookingClass": "J",
                        "cabinCode": "C",
                        "mealCode": "M",
                        "stopCount": 0,
                        "flightDuration": "2H 15Min"
                    }
                ]
            }
        ],
        "isRefundable": "Refundable"
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