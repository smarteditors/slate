## Authenticate

> `POST http://localhost:3000/api/v6/authenticate`

```ruby
example_params = {
  "user": {
    "email": String,
    "password": String
  }
}
```

> Example response

```json
{
  "success": true,
  "user": {
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
  },
  "status": 200
}
```

This endpoint authenticates a User.

### HTTP Request

`POST http://localhost:3000/api/v6/authenticate`

### Query Parameters

Parameter | Type | Description | Required?
--------- | ---- | ----------- | --------
email | String | A registered user email address | Yes
password | String | The user's password | Yes