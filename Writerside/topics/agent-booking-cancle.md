# Air Cancel

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/agent/booking/cancel{id}" method="delete">
    <request>
        <sample src="bookingUrl.json" include-lines="1-2"/>
    </request>
    <response type="200">
        <sample src="bookingSuccessSingle.json" include-lines="1-94"/>
    </response>
    <response type="400">
        <sample src="cancle.json" include-lines="1-4"/>
    </response>
    <response type="401">
        <sample src="unauthorized.json" include-lines="1-4"/>
    </response>
  <response type="404">
        <sample src="NotFoundRetrieve.json" include-lines="1-4"/>
    </response>
</api-endpoint>