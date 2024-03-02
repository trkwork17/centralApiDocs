# Routes and API Key Uses 

> access tokens information
>
> {style="note"}
### Token Generator


| Endpoint                           | Description                                                         |
|------------------------------------|---------------------------------------------------------------------|
| `/api_agent/get_access_token`      | Get the access token, to obtain an access token for live operations |
| `/api_agent/get_test_access_token` | Get the test access token for testing purposes.                     |


> Route Information
>
> {style="note"}

### Routes For Both Live and Test URL
| API Route                               | Description                                                                                                   |
|-----------------------------------------|---------------------------------------------------------------------------------------------------------------|
| `/booking/booking`                      | Create booking for one way, round way, and multi-city.                                                        |
| `/booking/retrieve_booking/{bookingId}` | Retrieve booking information for one way, round way, and multi-city air travel. By the provided `{bookingId}` |
| `/booking/cancel_booking/{bookingId}`   | Cancel a booking identified by the provided `{bookingId}`.                                                    |
| `/booking_history/:{bookingId}`         | Get full booking information.                                                                                 |
| `/booking/search-results`               | Make a search for one-way, round-trip, and multi-city flights.                                                |


 


