## Get Users

> `GET http://localhost:3000/api/v7/users`

> Example response

```json
{
  "request_id": "31be6f5e-45cd-4b9a-aa39-08eb843e72b4",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "users": [
    {
      "uuid": "8daf62d3-f86e-47bf-9c39-d7cb6babd0b5",
      "accepted_terms": false,
      "can_access_app": true,
      "can_access_web": true,
      "client_id": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
      "email": "ian@eastenders.com",
      "first_name": "Ian",
      "group": "user",
      "last_name": "Beale",
      "settings": null,
      "slug": "ian_beale",
      "token": "d76ee126-007b-44df-88f0-bd23add2583f",
      "username": "ian_beale"
    }
  ]
}
```

This endpoint retrieves all Users for the current client.

### HTTP Request

`GET http://localhost:3000/api/v7/users`