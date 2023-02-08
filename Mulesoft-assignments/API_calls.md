# Calling RESTful webservices
Make GET, DELETE, POST and PUT calls through a secured API proxy.

## Keyterminology
- Mocking service= 

## Assignment - Advanced REST Client(ARC)
GET requests.
- Send a get request using the http://training4-american-ws.cloudhub.io/api/flights link.
- Review the response and select RAW from the options in the response tab.
- Click the pencil infront of the request button to open the Parameter editor and click the Add button.
- Fill in the key and the value: destination - CLE.
- Click the send request button to receive responses only about CLE.
- Remove the parameter and refresh by requesting again.
- Change the link to http://apdev-american-ws.cloudhub.io/api/flights/3 by adding /3 in the link.
- Click the send request button to see what flight ID is being returned.

DELETE requests.
- Change method to DELETE.
- Press send request, you should see that the response returned deleted (though not really).
- Remove the URI parameter /3, giving you a 405 response.
- 'This is not allowed'

POST requests.
- Change method to Post and send the request again, giving you a 415 response of unsupported media type.
- Click add in the Header area set the key and value to: content-type and application/json.
- Select the Body tab and copy/paste the json code in the Body area.
- Click the send request to see the code 201 with: Flight added, but not really.
- Go to the Body area and remove the plane field and comma after the emptySeats key/value pair.
- Send the request; the message should still post successfully.
- Remove the emptySeats line and the comma after destination key/value pair.
- Sending request should get you the 400 response saying: Bad request.

PUT requests.
- Change method to PUT and add the flight ID /3 in the URL link.
- The response 400 should still appear, to fix this undo the changes up to the point that the emptySeats 
key/value pair is back in the body area.
- Send request again and a 200 response should appear with the message: Flight updated, but not really.

Make a request to a secured API.
- Remove the Content-type key/value pair in the Header area. 
- (don't forget to start fresh as continueing with the same URL at this point might give an error.)
- Change the URL link by exchanged the ws to api and change the method to GET.
- Sending the request should give the response 401 Unauthorized.
- Copy/paste the value of the client_id from the course snippets to the Header area, key/value being client_id/snippets value from the text file.
- Copy paste the key/value to the Header area, client_secret/snippets value from the text file.
- Click the send request and you should get the data for flight 3 again. With the response 200 which is positive!
- Keep sending requests till you get the response 429 for sending too many requests.

Using Mocking service.
- Go to https://anypoint.mulesoft.com/exchange/portals/muletraining/, select the American Flights API.
- Select /flights and select the GET method, review the review the headers and responses sections.
- On the right side you can select the server make sure its on Mocking service.
- Select LAX as destination in the Querry Parameter and fill in any value for the client_id and client_secret.
- When you send the request you should get example flights for SFO and ORD.
- Notice that the URL changes with the changes you set in the parameters.

Using API proxy Endpoint.
- Back at the top change the Mocking service to Rate limiting SLA based policy.
- Check the URL as seen before it changes with the changes you make.
- You get the response 401 Unauthorized again.
- Copy/paste the value of the client key's. key/value
- Sending the request after this should get you the response 200 that it is all Good.
