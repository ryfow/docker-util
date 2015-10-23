# Lightweight utilities in a Docker container

Based on Alpine Linux. Right now includes curl & jq.

# Usage:

Example of pulling github status page and finding "status" field
  alias JQ="docker run -i ryfow/util jq"
  alias CURL="docker run ryfow/util curl"
  CURL -s -L https://status.github.com/api/status.json | JQ .status


