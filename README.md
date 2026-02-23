# acme-relay
Relaying ACME HTTP requests to internal servers which handle ACME on their own. Is using public and private DNS for relaying based on Host-Header.

- Only handles port 80 HTTP requests and relays them into the internal network for specific URL-paths and host names
- .env file allows RegExp for allowed host names that get HTTP port 80 relayed to
- Validates source IPs, destination Host and URL-Path and GET method
- Single responsibility relay-reverse-proxy-server
- Uses Caddy Server (https://caddyserver.com/docs/caddyfile/concepts#structure)
