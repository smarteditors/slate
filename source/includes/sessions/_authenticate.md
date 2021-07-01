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