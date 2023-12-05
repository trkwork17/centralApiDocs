# Generate access token for perform operations

<!--If an operation has several responses, you can add samples for each of them separately.-->

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/user/createWithList" method="post">
    <response type="200">
        <sample lang="JSON">
        {
    "Success": true,
    "message": "Successfully get access token of agent",
    "data": Your access token
}
        </sample>
    </response>
<response type="400">
    <sample lang="JSON">
        {
    "success": false,
    "error": "Json Web Token is invalid, Try again"
}
    </sample>
</response>
</api-endpoint>
