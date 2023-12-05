# Booking MultiCity

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/api_agent/booking/multicitybooking" method="post">
    <request>
        <sample lang="JSON">
            {
  "platform": "QTB2B",
  "email": "dev@flyfar.tech",
  "phone": "1234567890",
  "name": "JohnDoe",
  "tripType": 3,
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
            "data": {
                "booking": {
                    "id": "37d5270220d543d7ac0c3d44453ced0c",
                    "uid": 452,
                    "bookingId": "QTBK1452",
                    "userId": null,
                    "vendor": "",
                    "invoice": "0.00",
                    "vendorCom": "0.00",
                    "ticketId": "",
                    "agentId": "c1d00d32551511eea7051831bf245c65",
                    "subagentId": null,
                    "staffId": null,
                    "email": "dev@flyfar.tech",
                    "phone": "1234567890",
                    "name": "JohnDoe",
                    "refundable": 1,
                    "upPnr": "",
                    "airlinesPNR": "6TN76V",
                    "tripType": "multiCity",
                    "journeyType": "Outbound",
                    "pax": 1,
                    "adultBag": "25 KG",
                    "childBag": "0",
                    "infantBag": "0",
                    "adultCount": 1,
                    "childCount": 0,
                    "infantCount": 0,
                    "currency": "BDT",
                    "buyPrice": 0,
                    "sellPrice": 0,
                    "clientCom": 0,
                    "paidAmount": 0,
                    "dueAmount": 0,
                    "wlagentCost": 0,
                    "subagentCost": 0,
                    "adultCostBase": 38786,
                    "childCostBase": 0,
                    "infantCostBase": 0,
                    "adultCostTax": 12742,
                    "childCostTax": 0,
                    "infantCostTax": 0,
                    "grossCost": 51528,
                    "baseFare": 38786,
                    "tax": 12742,
                    "netCost": 48580,
                    "ait": 0.003,
                    "coupon": "",
                    "bonus": "",
                    "additionalMarkupWL": 0,
                    "additionalMarkupB2B": 0,
                    "deptFrom": "Dhaka",
                    "airlines": "",
                    "airlinesComRef": "",
                    "airlinesCode": "",
                    "commissionType": "sabresitti",
                    "commissionValue": "8",
                    "arriveTo": "Singapore",
                    "gds": "",
                    "flightNo": "",
                    "bookingClass": "",
                    "status": "Hold",
                    "isPartial": "",
                    "PPStatus": "",
                    "travelDate": "2024-02-01T07:40:00.000Z",
                    "timeLimit": "06-12-23T23:00",
                    "searchId": "",
                    "resultId": "",
                    "bookedBy": "",
                    "maker": "",
                    "platform": "QTB2B",
                    "gdsSegment": "",
                    "ticketCoupon": "",
                    "lossAmount": "0.00",
                    "itaNumber": "",
                    "pccNumber": "",
                    "remarks": "",
                    "lossReason": "",
                    "lossProfitCom": "0.00",
                    "assign": null,
                    "assignBy": "agent",
                    "assignTime": "2023-12-02T11:04:26.000Z",
                    "paidDate": "2023-12-02T11:04:06.000Z",
                    "dueDate": "2023-12-02T11:04:06.000Z",
                    "bookedAt": "2023-12-02T11:04:06.000Z",
                    "timeUpdateBy": "agent",
                    "lastUpdated": "2023-12-02T11:04:26.000Z",
                    "adminId": null
                },
                "Passengers": [
                    {
                        "id": "40766c7f1b0e40b78df59a77f55091ed",
                        "uid": 960,
                        "paxId": "QTP1960",
                        "agentId": "c1d00d32551511eea7051831bf245c65",
                        "subagentId": null,
                        "staffId": null,
                        "bookingId": "37d5270220d543d7ac0c3d44453ced0c",
                        "userId": "",
                        "prefix": "MR",
                        "firstName": "wekdtest",
                        "lastName": "mncytest",
                        "dob": "1997-11-01",
                        "type": "ADT",
                        "passNation": "BD",
                        "passNo": "419965",
                        "passEx": "2023-12-02T11:04:29.000Z",
                        "phone": "",
                        "email": "",
                        "address": "",
                        "gender": "Male",
                        "passportCopy": "",
                        "visaCopy": "",
                        "createdAt": "2023-12-02T11:04:07.000Z",
                        "updatedAt": "2023-12-02T11:04:29.000Z",
                        "adminId": null
                    }
                ]

    ]
}

            
</sample>    
    </response>
    <response type="401">
        <sample lang="JSON">
            {
  "success": false,
  "error": "No authorization token was found"
}   
      </sample>      
    </response>
  <response type="404">
         <sample lang="JSON">
           {
  "success": false,
  "error": "No fights found"
}
      </sample>   
    </response>
</api-endpoint>