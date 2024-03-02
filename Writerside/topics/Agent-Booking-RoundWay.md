# Booking Round Way

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/api_agent/booking/roundbooking" method="post">
    <request>
         <sample lang="JSON">
            {
  "platform": "QTB2B",
  "email": "dev@flyfar.tech",
  "phone": "1234567890",
  "name": "JohnDoe",
  "tripType": "2",
  "passengerData": {
    "adult": [
      {
        "firstName": "karilmtest",
        "lastName": "krtest",
        "gender": "Male",
        "dob": "1997-11-01",
        "passNation": "BD",
        "passNo": "413449965",
        "passEx": "2026-11-20",
        "type": "ADT",
        "prefix": "MR"
      }
    ],
    "child": [],
    "infant": []
  },
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
} 
      </sample>   
    </request>
    <response type="200">
          <sample lang="JSON">
{
    "success": true,
    "message": "Booking create successfully ",
    "data": [
        {
            "booking": {
                "id": "dd2ab1740f8b4b239a81d07b43c0e74f2",
                "bookingId": "QTBK1497"
            }
        }
    ]
}
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