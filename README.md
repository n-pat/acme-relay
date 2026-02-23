# acme-relay
Relaying ACME HTTP requests to internal servers which handle ACME on their own. Is using public and private DNS for relaying based on Host-Header.

- Only handles port 80 HTTP requests
- Single responsibility relay-reverse-proxy-server
- Validates source IPs, destination Host and URL-Path
