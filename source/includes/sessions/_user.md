## User

> `GET http://localhost:3000/api/v6/sessions/user`

> Example response

```json
{
  "success": true,
  "user": {
    "id": 1,
    "first_name": "sergio",
    "last_name": "mmmmmm",
    "username": "sergiomarrocoli",
    "token": "hello",
    "email": "sergio@smarteditors.co.uk",
    "slug": "sergiomarrocoli",
    "uuid": "5656d494-b4f8-4ee9-a48d-d3286d954a45",
    "created_at": "2020-11-09T13:12:25.000+00:00",
    "updated_at": "2021-06-17T14:46:25.000+01:00",
    "settings": null,
    "group": "user",
    "accepted_terms": true,
    "client_id": 6,
    "can_access_web": true,
    "can_access_app": true
  },
  "status": 200
}
```

This endpoint returns the current User.

### HTTP Request

`GET http://localhost:3000/api/v6/sessions/user`