# Access Token


<api-endpoint openapi-path="./../openapi.yaml" endpoint="/get_access_token" method="get">
  <response type="200">
         <sample lang="JSON">
        {
    "Success": true,
    "message": "Successfully get access token of agent",
    "data": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImZvdW5kZXJAZmx5ZmFybGFkaWVzLmNvbSIsImlkIjoiYTJlOTE1YjM5NjE3NDllNThlYzc3YjcxYjk1YWIwNWUiLCJ0b2tlbiI6ImV5SmhiR2NpT2lKSVV6STFOaUlzSW5SNWNDSTZJa3BYVkNKOS5leUpsYldGcGJDSTZJbVp2ZFc1a1pYSkFabXg1Wm1GeWJHRmthV1Z6TG1OdmJTSXNJbWxrSWpvaVlUSmxPVEUxWWpNNU5qRTNORGxsTlRobFl6YzNZamN4WWprMVlXSXdOV1VpTENKcFlYUWlPakUzTURFMk9EVTNOVEI5LlY3d2FnaHVZaW9FSFg3RG0wdGtrWkNZcmFST1BUUmJVd2swZzVXbEE1ckEiLCJpYXQiOjE3MDE3NzM5NDMsImV4cCI6MTcwMTk0Njc0M30.biRp6LFVZvQPKbI-W0SJvtCvrjgTTFwdywJs-DO6Nh4"
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