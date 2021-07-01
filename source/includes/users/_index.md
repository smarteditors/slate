## Get Users

> `GET http://localhost:3000/api/v6/users`

> Example response

```json
[
  {
    "uuid": "5656d494-b4f8-4ee9-a48d-d3286d954a45",
    "first_name": "ian",
    "last_name": "beale",
    "username": "ianbeale",
    "token": "token",
    "email": "ian@eastenders.com",
    "slug": "ianbeale",
    "settings": null,
    "group": "user",
    "accepted_terms": true,
    "can_access_web": true,
    "can_access_app": true
  }
]
```

This endpoint retrieves all Users for the current client.

### HTTP Request

`GET http://localhost:3000/api/v6/users`