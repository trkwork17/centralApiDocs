# Booking one Way

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/agent/booking/booking" method="post">
    <request>
        <sample src="oneWay.json" include-lines="1-37"/>
    </request>
    <response type="200">
        <sample src="oneWaySuccess.json" include-lines="1-122"/>
    </response>
    <response type="401">
        <sample src="unauthorized.json" include-lines="1-4"/>
    </response>
  <response type="404">
        <sample src="NotFound.json" include-lines="1-4"/>
    </response>
</api-endpoint>