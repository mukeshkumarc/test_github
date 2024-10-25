### GET /api/v1/resource

**Description**  
Retrieves a list of resources.

**Request**
- **URL**: `/api/v1/resource`
- **Method**: `GET`
- **Headers**:
  - `Authorization`: Bearer token required
  - `Content-Type`: `application/json`
- **Parameters**:
  - **query (optional)**: A search term to filter results
  - **limit (optional)**: Number of results to return, default is 20

**Response**:
- **200 OK**:
  ```json
  {
    "data": [
      {
        "id": 1,
        "name": "Example Resource",
        "description": "This is an example resource."
      }
    ],
    "meta": {
      "count": 1
    }
  }

