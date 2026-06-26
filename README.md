# Local Evolution API

```sh
# Clone repo
git clone <url> local-evolution-api \
  cd local-evolution-api

# start
docker compose -f ./docker-compose.local.yaml up -d

# Browser
# http://localhost:8080/manager

# API KEY - changeme

# Create an instance, required fields:
# - Name (preference without spaces)
# - Select Bayles
# - Country code + DDD + number, e.g., 5519999999999

# Send message
# Endpoint: http://localhost:8080/message/sendText/<instance_name>
# Authentication: apiKey=<instance_api_key>
# Body (JSON): { "number": "<destiny>", "text": "something" }

# Down containers
docker compose -f ./docker-compose.local.yaml down -v
```
