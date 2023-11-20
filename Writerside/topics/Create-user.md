# Create Agent Account

<!--Specify request and response samples manually. 
You can add the sample inside the <sample> element or include it from a file using the 'src' attribute.-->

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/agent/create_agent" method="post">
    <request>
        <sample src="examples.json" include-lines="1-10"/>
    </request>
    <response type="default">
        <sample>
{
    "success": true,
    "message": "We are verifying Your Account Please Wait ",
    "data": {
        "id": "1a4e74e109a749fd95903ee8ccea0158",
        "uid": 11,
        "agentId": "QTA1011",
        "firstName": "ab",
        "lastName": "d21",
        "email": "abc333@gmail.com",
        "phone": "+880123456789",
        "joinAt": "2023-10-08T04:16:00.000Z",
        "status": "pending",
        "isActive": 1,
        "company": "aaa1",
        "companyAdd": "bd",
        "area": "",
        "companyImage": "http://localhost:5000/public/uploads/Screenshot-2023-08-28-154000.png-1696738560244.webp",
        "visaMarkupType": "",
        "visaMarkup": "",
        "markup": "",
        "bonusId": null,
        "credit": null,
        "creditBy": null,
        "loginIp": "::1",
        "browser": "Other 0.0.0",
        "platform": "Other 0.0.0",
        "website": "",
        "approvedBy": null
    }
}
        </sample>
    </response>
</api-endpoint>
