
# VPN and Proxy Connection Checker API

This API allows you to check if a visitor's connection is coming from a VPN or proxy server. By simply sending a GET request to the provided endpoint with the visitor's IP address, you can quickly determine if they are using such services.

## How to Use

To check if a visitor's connection is from a VPN or proxy server, send a GET request to the following endpoint:

```
https://vpnjobdastak.kozow.com:3000/?ip={VISITOR_IP_HERE}
```

Replace `{VISITOR_IP_HERE}` with the IP address of the visitor whose connection you want to check.

### Example

```
https://vpnjobdastak.kozow.com:3000/?ip=8.8.8.8
```

This will return a response indicating whether the IP address belongs to a VPN or proxy connection.

## Response Format

The API will return a JSON response with the following format:

```json
{
  "ip": "123.456.789.012",
  "is_vpn": true,
  "is_proxy": false
}
```

- `ip`: The IP address that was checked.
- `is_vpn`: Indicates whether the IP address belongs to a VPN connection (`true` or `false`).
- `is_proxy`: Indicates whether the IP address belongs to a proxy connection (`true` or `false`).

## Usage Limits

Please note that there might be usage limits or rate limiting in place for this API. Make sure to check the documentation or contact the provider for more information.

## Disclaimer

This API is provided for informational purposes only. While it can help identify VPN or proxy connections, it may not be 100% accurate in all cases. Use it responsibly and consider additional security measures as needed.

---

Feel free to customize this README with additional information such as installation instructions, examples of use, or any other relevant details about your API. Let me know if you need further assistance!
