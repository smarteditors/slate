## Get Users

```shell
curl "http://localhost:3000/api/v6/users" \
  -H "token: meowmeowmeow"
```

> The above command returns JSON structured like this:

```json
[
    {
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
    {
        "id": 2,
        "first_name": "mmm",
        "last_name": "mmm",
        "username": "mmm mmm",
        "token": null,
        "email": "sergio2@smarteditors.co.uk",
        "slug": "mmm-mmm",
        "uuid": "8daf62d3-f86e-47bf-9c39-d7cb6babd0b5",
        "created_at": "2021-03-15T10:59:18.000+00:00",
        "updated_at": "2021-06-17T14:45:48.000+01:00",
        "settings": null,
        "group": "user",
        "accepted_terms": false,
        "client_id": 1,
        "can_access_web": true,
        "can_access_app": true
    }
]
```

This endpoint retrieves all Users for the current client.

### HTTP Request

`GET http://localhost:3000/api/v6/users`