# HNG12numberAPI
## Number Classification API

It's me again, back with another API. This API classifies numbers based on mathematical properties, it returns fun facts about a number whether it is even, odd, armstrong, prime, perfect and so on. Way to deal with numbers right.

## Features
- Checks if a number is prime or perfect.
- Determines if a number is odd or even.
- Identifies Armstrong numbers.
- Fetches a fun fact using the Numbers API.

## Endpoint
*GET* /api/classify-number?number=<integer>

## Example Usage
- Using a web browser
Open your web browser, in the address bar, enter the following URL
[hng12numberapi.onrender.com/api/classify-number?number=7], you can replace 7 with any integer.

The browser will display the JSON response, which would look something like this 

```json
{
  "number": 7,
  "is_prime": true,
  "is_perfect": false,
  "properties": [
    "armstrong",
    "odd"
  ],
  "digit_sum": 7,
  "fun_fact": "7 is the lowest number that cannot be represented as the sum of the squares of three integers."
}
```

If you enter a non-numeric value, such as
[hng12numberapi.onrender.com/api/classify-number?number=hi] 

The response should be:

```json
{
    "number": "hi",
    "error": true,
    "message": "Input should be a valid integer"
}
```