# Booking one Way

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/api_agent/booking/booking" method="post">
    <request>
        <sample lang="JSON">
            {
  "platform": "QTB2B",
  "email": "dev@flyfar.tech",
  "phone": "1234567890",
  "name": "JohnDoe",
  "tripType": "1",
 "searchId": "7ec262888afc4d2c8e308c31a326aeb8",
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
            "marketingCarrier": "QR",
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
 {
    "success": true,
    "message": "Booking create successfully ",
    "data": [
        {
            "booking": {
                "id": "dd2ab1740f8b4b239a81d07b43c0e74f1",
                "bookingId": "QTBK1496"
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