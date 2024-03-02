# Booking MultiCity

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/api_agent/booking/multicitybooking" method="post">
    <request>
        <sample lang="JSON">
            {
  "platform": "QTB2B",
  "email": "dev@flyfar.tech",
  "phone": "1234567890",
  "name": "JohnDoe",
  "tripType": "3",
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
  "segments": [
        {
            "marketingCarrier": "TG",
            "marketingFlightNumber": 322,
            "operatingCarrier": "TG",
            "operatingFlightNumber": 322,
            "departure": "DAC",
            "departureDateTime": "2024-02-01T13:40:00",
            "arrival": "BKK",
            "arrivalDateTime": "2024-02-01T17:10:00",
            "bookingClass": "V"
        },
        {
            "marketingCarrier": "TG",
            "marketingFlightNumber": 401,
            "operatingCarrier": "TG",
            "operatingFlightNumber": 401,
            "departure": "BKK",
            "departureDateTime": "2024-02-05T19:40:00",
            "arrival": "SIN",
            "arrivalDateTime": "2024-02-05T23:00:00",
            "bookingClass": "V"
        }
    ]
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
                "id": "dd2ab1740f8b4b239a81d07b43c0e74f",
                "bookingId": "QTBK1498"
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