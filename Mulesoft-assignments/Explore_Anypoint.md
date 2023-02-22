# Explore Anypoint Platform
- Explore Anypoint Platform.
- BrowseAnypoint Exchange.
- Review an API portal for a REST API in Exchange.
- Discover and make calls tothe Training: American Flights APIin the public Exchange.

## Keyterminology

## Assignment
Return to Anypoint Platform
- Go to the Anypoint Platform following this link: https://anypoint.mulesoft.com/home/organizations/7b637aa9-78a9-46a0-80dc-2f05a5b29387/
- The main menu is the Anypoint Platform homepage.

Explore Anypoint Platform
- In the main menu (the menu from the homepage in the left topcorner), select Design Center.
- Click the Create new button and look at the options in the popup.
- In the main menu, select Runtime Manager.
- If you get a Choose Environment page, select Design.
- In the main menu, select API Manager.

Explore Anypoint Exchange
- In the main menu, select Exchange.
- In the left-side navigation, selectProvided by MuleSoft; you should see all the content in the public Exchange.
- In the left-side navigation, selectthe name of your organization above Provided by MuleSoft(Training in the screenshots); 
  you should now see only the content in your private Exchange, which is currently empty.
- In the left-side navigation, selectProvided by MuleSoft.
- In the types menu, select Connectors.
- Select one of the connectors and review its information.
- In the left-side navigation, click the Assets list link.
- Enter salesforce into the search field and press Enter/Return.
- LocatetheSalesforce Connector-Mule 4 connector and review its details.
- In the left-side navigation, click Assets list.
- In the types menu, select Templates.
- Remove salesforce from the search field and press Enter/Return.

Browse REST API's in Anypoint Exchange
- In the types menu, select REST APIs.
- Browse the APIs.

Browse the American Flights API
- Click Try the new search and examine the new search features available in Exchange.
- Locate and click the Training: American Flights API.
- Review the API portal.
- In the left-side navigation, expand and review the list of available resources.
- Click the GET link for the /flightsresource.
- On the GET /flightspage, review the information for the optional destination 
  query parameter; you should see the API is similar to the one you explored in 
  the public MuleSoft Training portal.

Making calls to American Flights API
- In the API console, review the options for the instances you can test.
- Select Mocking Service.
- Select a destination in the drop-down menu.
- In the Headers section, enter any values for client_id and client_secret.
- Click Send; you should get the two example flights.
- Change the API instance from Mocking Service to Rate limiting SLA based policy.
- Select a destination in the drop-down menu.
- In the Headers section, copy and paste the client_id and client_secret values from the course snippets.txt file.
- Click Send again; you should get results from the actual API implementation for the destination you selected.

## Sources
