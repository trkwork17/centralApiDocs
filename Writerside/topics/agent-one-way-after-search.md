# one Way After Search


<api-endpoint openapi-path="./../openapi.yaml" endpoint="/api_agent/booking/search-results" method="get">
<request>
        <sample lang="JSON">
          {
  "type": "oneway",
  "departureDate": "2023-12-15",
  "departure": "DAC",
  "arrival": "DXB",
  "adultCount": 1,
  "childCount": 0,
  "infantCount": 0,
  "cabin": "Economy"
}
      </sample>      
    </request> 
  <response type="200">
         <sample lang="JSON">
       {
        "uId": "da7f3eea0de14f04823897c4926dc31f",
        "system": "system001",
        "segment": 1,
        "tripType": "Outbound",
        "carrier": "BG",
        "carrierName": "Biman Bangladesh Airlines",
        "lastTicketedTime": "2023-12-12 23:59",
        "basePrice": 82875,
        "taxes": 9268,
        "agentPrice": 92143,
        "clientPrice": 92143,
        "commission": 0,
        "commissionValue": 0,
        "commissionType": "sitti",
        "departure": "DAC",
        "departureDate": "2023-12-31",
        "departureTime": "20:35",
        "arrival": "DXB",
        "arrivalDate": "2024-01-01",
        "arrivalTime": "00:20",
        "class": "Business",
        "fareCurrency": "BDT",
        "totalFlightDuration": "5H 45Min",
        "transit": {
            "Transit": "0"
        },
        "availableSeat": "8",
        "baggage": "40 KG",
        "priceBreakdown": [
            {
                "paxType": "ADT",
                "paxCount": 1,
                "baseFare": 82875,
                "totalBaseFare": 82875,
                "Tax": 9268,
                "totalTaxAmount": 9268,
                "totalAmount": 92143,
                "discount": 0,
                "otherCharges": 0,
                "serviceFee": 0
            }
        ],
        "segments": [
            {
                "aircraft": "BOEING 787-8",
                "marketingCarrier": "BG",
                "marketingCarrierName": "Biman Bangladesh Airlines",
                "marketingFlight": "347",
                "operatingCarrier": "BG",
                "operatingCarrierName": "Biman Bangladesh Airlines",
                "operatingFlight": "347",
                "departure": "DAC",
                "departureAirport": "Hazrat Shahjalal Intl Airport",
                "departureLocation": "Dhaka,Bangladesh",
                "departureCity": "Dhaka",
                "departureCountryCode": "BD",
                "departureCountryName": "BANGLADESH",
                "departureDate": "2023-12-31",
                "departureTime": "20:35",
                "departureDateTime": "2023-12-31T20:35",
                "arrival": "DXB",
                "arrivalAirport": "Dubai Intl Airport",
                "arrivalLocation": "Dubai,UNITED ARAB EMIRATES",
                "arrivalCity": "Dubai",
                "arrivalCountryCode": "AE",
                "arrivalCountryName": "UNITED ARAB EMIRATES",
                "arrivalDate": "2024-01-01",
                "arrivalDateTime": "2024-01-01T00:20",
                "arrivalTime": "2024-01-01",
                "flightDuration": "5H 45Min",
                "bookingClass": "D",
                "cabinCode": "C",
                "mealCode": "S",
                "seatAvailable": "8",
                "baggage": "40 KG"
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