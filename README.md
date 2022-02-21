# okhttp3-log-retry-and-followup-requests

A Frida script to log okhttp3 http(s) communication.

Targeted application must use RetryAndFollowUpInterceptor, which this script
overloads. 

By default uses `console.log()`. If an error is caught during processing, uses
`console.warn()`.

Requests and responses are by default formatted with JSON.stringify().

Additionally accepts parameters:

`{"format": "text"}` - output is formated in curl-like text

`{"raw": true}` - includes representation of original request and response
objects

## License

MIT
