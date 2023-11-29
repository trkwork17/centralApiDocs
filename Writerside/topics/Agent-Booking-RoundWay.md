# Booking Round Way

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/agent/booking/roundbooking" method="post">
    <request>
        <sample src="roundWay.json" include-lines="1-54"/>
    </request>
    <response type="200">
        <sample src="roundWaySuccess.json" include-lines="1-122"/>
    </response>
    <response type="401">
        <sample src="unauthorized.json" include-lines="1-4"/>
    </response>
  <response type="404">
        <sample src="NotFound.json" include-lines="1-4"/>
    </response>
</api-endpoint>