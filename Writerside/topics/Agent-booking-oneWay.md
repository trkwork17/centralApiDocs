# Booking one Way

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/api_agent/booking/booking" method="post">
    <request>
        <sample lang="JSON">
            {
  "platform": "QTB2B",
  "email": "dev@flyfar.tech",
  "phone": "1234567890",
  "name": "JohnDoe",
  "tripType": 1,
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
      "marketingCareer": "BS",
      "marketingFlight": "142",
      "operatingCareer": "BS",
      "operatingFlight": "142",
      "departure": "CXB",
      "departureDateTime": "2023-12-25T09:20:00",
      "arrival": "DAC",
      "arrivalDateTime": "2023-12-25T10:20:00",
      "bookingCode": "I"
    }
  ]
} 
      </sample>      
    </request>
    <response type="200">
         <sample lang="JSON">
           [
  {
    "data": {
      "booking": {
        "id": "917a5bd4a54e4aeb82413d9428afdd47",
        "uid": 376,
        "bookingId": "QTBK1376",
        "userId": null,
        "vendor": "",
        "invoice": "0.00",
        "vendorCom": "0.00",
        "ticketId": "",
        "agentId": "c1d00d32551511eea7051831bf245c65",
        "subagentId": null,
        "staffId": null,
        "email": "sakhawat@flyfar.tech",
        "phone": "1234567890",
        "name": "John",
        "refundable": 1,
        "upPnr": "",
        "airlinesPNR": "55PT6O",
        "tripType": "oneWay",
        "journeyType": "Outbound",
        "pax": 3,
        "adultBag": "2 Piece",
        "childBag": "2 Piece",
        "infantBag": "1 Piece",
        "adultCount": 1,
        "childCount": 1,
        "infantCount": 1,
        "currency": "BDT",
        "buyPrice": "0.00",
        "sellPrice": "0.00",
        "clientCom": "0.00",
        "paidAmount": "0.00",
        "dueAmount": "0.00",
        "wlagentCost": "0.00",
        "subagentCost": "0.00",
        "adultCostBase": "68842.00",
        "childCostBase": "52267.00",
        "infantCostBase": "13260.00",
        "adultCostTax": "19024.00",
        "childCostTax": "16024.00",
        "infantCostTax": "7652.00",
        "grossCost": "177069.00",
        "baseFare": "134369.00",
        "tax": "42700.00",
        "netCost": "177069.00",
        "ait": 0,
        "coupon": "",
        "bonus": "",
        "additionalMarkupWL": "0.00",
        "additionalMarkupB2B": "0.00",
        "deptFrom": "DAC",
        "airlines": "Kuwait Airways",
        "airlinesComRef": "",
        "airlinesCode": "KU",
        "commissionType": "sabresotto",
        "commissionValue": "0",
        "arriveTo": "JFK",
        "gds": "",
        "flightNo": "",
        "bookingClass": "",
        "status": "Hold",
        "isPartial": "",
        "PPStatus": "",
        "travelDate": "2023-12-16T19:25:00.000Z",
        "timeLimit": "24-11-23T12:57",
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
        "assignTime": "2023-11-22T08:58:02.000Z",
        "paidDate": "2023-11-22T08:57:44.000Z",
        "dueDate": "2023-11-22T08:57:44.000Z",
        "bookedAt": "2023-11-22T08:57:44.000Z",
        "timeUpdateBy": "agent",
        "lastUpdated": "2023-11-22T08:58:02.000Z",
        "adminId": null
      },
      "Passengers": [
        {
          "id": "253173eafe5b4b79ba022aaec7b2314b",
          "uid": 813,
          "paxId": "QTP1813",
          "agentId": "c1d00d32551511eea7051831bf245c65",
          "subagentId": null,
          "staffId": null,
          "bookingId": "917a5bd4a54e4aeb82413d9428afdd47",
          "userId": "",
          "prefix": null,
          "firstName": "Kabirt",
          "lastName": "Khant",
          "dob": "1997-11-20",
          "type": "",
          "passNation": "BD",
          "passNo": "12345432123",
          "passEx": "2023-11-22T08:58:03.000Z",
          "phone": "",
          "email": "",
          "address": "",
          "gender": "Male",
          "passportCopy": "",
          "visaCopy": "",
          "createdAt": "2023-11-22T08:57:45.000Z",
          "updatedAt": "2023-11-22T08:58:03.000Z",
          "adminId": null
        }
      ]
    }
  }
]
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