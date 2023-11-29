# Air Price round Way

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/agent/booking/air-price-roundWay" method="post">
    <request>
        <sample src="roundWayPrice.json" include-lines="1-57"/>
    </request>
    <response type="200">
        <sample src="priceSuccess.json" include-lines="1-38"/>
    </response>
    <response type="401">
        <sample src="unauthorized.json" include-lines="1-4"/>
    </response>
  <response type="404">
        <sample src="NotFound.json" include-lines="1-4"/>
    </response>
</api-endpoint>