## Logout

> `DELETE http://localhost:3000/api/v7/sessions/logout`

> Example response

```json
{
  "request_id": "2bbfaff1-5cb7-4599-ac9f-7c45e71859f5",
  "authority": {
    "email": null
  },
  "message": "User is logged out."
}
```

This endpoint logs out a user.

### HTTP Request

`DELETE http://localhost:3000/api/v7/sessions/logout`