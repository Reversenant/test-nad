# API Reference

## `Client`

### `Client(base_url: str = "https://api.example.com")`
Creates a new client instance.

### `request(endpoint: str, method: str = "GET", data: dict = None) -> dict`
Sends a request to the specified endpoint.

#### Example:

```python
client.request("/status")