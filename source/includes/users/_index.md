## Get Users

> `GET http://localhost:3000/api/v6/users`

> Example response

```json
[
  {
    "id": 1,
    "first_name": "ian",
    "last_name": "beale",
    "username": "ianbeale",
    "token": "token",
    "email": "ian@eastenders.com",
    "slug": "ianbeale",
    "uuid": "5656d494-b4f8-4ee9-a48d-d3286d954a45",
    "created_at": "2020-11-09T13:12:25.000+00:00",
    "updated_at": "2021-06-17T14:46:25.000+01:00",
    "settings": null,
    "group": "user",
    "accepted_terms": true,
    "client_id": 6,
    "can_access_web": true,
    "can_access_app": true
  }
]
```

This endpoint retrieves all Users for the current client.

### HTTP Request

`GET http://localhost:3000/api/v6/users`