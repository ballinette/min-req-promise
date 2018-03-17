# Minimal Request Promise

[`request`](https://www.npmjs.com/package/request) and [`request-promise`](https://www.npmjs.com/package/request-promise) are great, but I was looking for an some extra-light implementation.

## Usage

```
const client = require('minimal-request-promise');

return client.get('https://some/url')
  .then(response => {
    // response is an http.IncomingMessage
    // with an extra `body` member
    
    console.log(response.headers);
    console.log(response.body);
  });
```
