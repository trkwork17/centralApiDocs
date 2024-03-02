# Access Token Test

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/get_test_access_token" method="get">
  <response type="200">
         <sample lang="JSON">
       {
    "Success": true,
    "message": "Successfully get test access token of agent",
    "data": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImZvdW5kZXJAZmx5ZmFybGFkaWVzLmNvbSIsImlkIjoiYTJlOTE1YjM5NjE3NDllNThlYzc3YjcxYjk1YWIwNWUiLCJpYXQiOjE3MDkxOTQ5MjcsImV4cCI6MTcwOTM2NzcyN30.KcP6i9f8hxtxUitYjotW-PYKgdL6Tz9pT81g0n2XC4U"
}
      </sample>    
    </response>
 <response type="400">
         <sample lang="JSON">
           {
 {
    "success": false,
    "error": "Json Web Token is invalid, Try again"
}
      </sample>   
    </response>
<response type="404">
        <sample lang="JSON">
            {
  "success": false,
  "error": "No authorization token was found"
}   
      </sample>      
    </response>

</api-endpoint>