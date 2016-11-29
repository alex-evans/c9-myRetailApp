# 1. myRetail RESTful service

## User Stories
- Responds to an HTTP GET request at /products/{id} and delivers product data as JSON (where {id} will be a number)
-- Example product IDs: 15117729, 16483589, 16696652, 16752456, 15643793)
-- Example response: {"id":13860428,"name":"The Big Lebowski (Blu-ray) (Widescreen)","current_price":{"value":13.49,"currency_code":"USD"}}
- Performs an HTTP GET to retrieve the product name from an external API.
- Reads pricing information from a NoSQL data store and combines it with the product id and name from the HTTP request into a single response
- BONUS: Accepts an HTTP PUT request at the same path (/products/{id}), containing a JSON request body similar to the GET response, and updates the product's price in the data store
