## Authenticate

> `POST https://smartedi2.smarteditors.co.uk/api/v7/sessions/authenticate`

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
  "request_id": "6d9afa34-9e1d-49f0-a384-e3d610bfc242",
  "authority": {
    "email": null
  },
  "user": {
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
}
```

This endpoint authenticates a User. Once authenticated endpoints can be accessed provided a valid token is submitted in the request header.

### HTTP Request

`POST https://smartedi2.smarteditors.co.uk/api/v7/sessions/authenticate`

### Query Parameters

Parameter | Type | Description | Required?
--------- | ---- | ----------- | --------
email | String | A registered user email address | Yes
password | String | The user's password | Yes