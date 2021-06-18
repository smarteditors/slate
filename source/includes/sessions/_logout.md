## Logout

```ruby
api = EDi::APIClient
api.sessions.logout
```

> The above command returns JSON structured like this:

```json
{
  "success": true,
  "message": "",
  "status": 200
}
```

This endpoint logs out a user.

### HTTP Request

`DELETE http://localhost:3000/api/v6/sessions/logout`