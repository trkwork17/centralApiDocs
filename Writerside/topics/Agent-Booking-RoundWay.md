# Booking Round Way

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/api_agent/booking/roundbooking" method="post">
    <request>
         <sample lang="JSON">
            {
  "platform": "QTB2B",
  "email": "dev@flyfar.tech",
  "phone": "1234567890",
  "name": "JohnDoe",
  "tripType": 2,
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
        "marketingCareer": "BS",
        "marketingFlight": 341,
        "operatingCareer": "BS",
        "operatingFlight": 341,
        "departure": "DAC",
        "departureDateTime": "2023-12-10T17:00:00",
        "arrival": "DXB",
        "arrivalDateTime": "2023-12-10T20:45:00",
        "bookingCode": "E"
      }
    ],
    "back": [
      {
        "marketingCareer": "BS",
        "marketingFlight": 342,
        "operatingCareer": "BS",
        "operatingFlight": 342,
        "departure": "DXB",
        "departureDateTime": "2023-12-10T21:45:00",
        "arrival": "DAC",
        "arrivalDateTime": "2023-12-20T04:20:00",
        "bookingCode": "E"
      }
    ]
  }
} 
      </sample>   
    </request>
    <response type="200">
          <sample lang="JSON">
         [
  {
    "data": {
      "booking": {
        "id": "2ed1c42aa21f4e5c9ac67018e94db0a0",
        "uid": 300,
        "bookingId": "QTBK1300",
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
        "name": "skr",
        "refundable": 1,
        "upPnr": "",
        "airlinesPNR": "NNPCAE",
        "tripType": "oneWay",
        "journeyType": "Outbound",
        "pax": 1,
        "adultBag": "20 KG",
        "childBag": "0",
        "infantBag": "0",
        "adultCount": 1,
        "childCount": 0,
        "infantCount": 0,
        "currency": "BDT",
        "buyPrice": "0.00",
        "sellPrice": "0.00",
        "clientCom": "0.00",
        "paidAmount": "0.00",
        "dueAmount": "0.00",
        "wlagentCost": "0.00",
        "subagentCost": "0.00",
        "adultCostBase": "8050.00",
        "childCostBase": "0.00",
        "infantCostBase": "0.00",
        "adultCostTax": "1950.00",
        "childCostTax": "0.00",
        "infantCostTax": "0.00",
        "grossCost": "10000.00",
        "baseFare": "8050.00",
        "Tax": "1950.00",
        "netCost": "10000.00",
        "ait": 0,
        "coupon": "",
        "bonus": "",
        "additionalMarkupWL": "0.00",
        "additionalMarkupB2B": "0.00",
        "deptFrom": "DAC",
        "airlines": "Biman Bangladesh Airlines",
        "airlinesComRef": "",
        "airlinesCode": "BG",
        "commissionType": "sabresotto",
        "commissionValue": "0",
        "arriveTo": "DAC",
        "gds": "",
        "flightNo": "",
        "bookingClass": "",
        "status": "Hold",
        "isPartial": "",
        "PPStatus": "",
        "travelDate": "2023-12-03T08:45:00.000Z",
        "timeLimit": "/RKBST//FBGCEST.COM",
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
        "assignTime": "2023-11-19T04:38:35.000Z",
        "paidDate": "2023-11-19T04:38:22.000Z",
        "dueDate": "2023-11-19T04:38:22.000Z",
        "bookedAt": "2023-11-19T04:38:22.000Z",
        "timeUpdateBy": "agent",
        "lastUpdated": "2023-11-19T04:38:35.000Z",
        "adminId": null
      },
      "Passengers": [
        {
          "id": "ff1ed9d0c4254d6384ec61f7578f4d96",
          "uid": 710,
          "paxId": "QTP1710",
          "agentId": "c1d00d32551511eea7051831bf245c65",
          "subagentId": null,
          "staffId": null,
          "bookingId": "2ed1c42aa21f4e5c9ac67018e94db0a0",
          "userId": "",
          "prefix": null,
          "firstName": "rkbst",
          "lastName": "fbgcest",
          "dob": "2003-09-06",
          "type": "",
          "passNation": "BD",
          "passNo": "201212ACF",
          "passEx": "2023-11-19T04:38:36.000Z",
          "phone": "",
          "email": "",
          "address": "",
          "gender": "Male",
          "passportCopy": "",
          "visaCopy": "",
          "createdAt": "2023-11-19T04:38:23.000Z",
          "updatedAt": "2023-11-19T04:38:36.000Z",
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