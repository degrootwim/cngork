# Getting started with cngrok and docker-compose.

```yaml
version: "3.3"

services:
  tunnel:
    image: wimdegroot/cngrok
    environment:
      - AUTH_TOKEN=aduiflhewor2q9h92lbEXAMPLE
      - PROTOCOL=http
      - PORT=80
      - SUBDOMAIN=subdomain
      - REGION=eu
      - ADDRESS=http://some-service
  some-service:
    # some-service config ...
```
