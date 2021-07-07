## Get All Action Stamps

```ruby
api = EDi::APIClient
api.stamps
```

> Example response

```json
[
  "anew",
  "estate_reused",
  "estate_reused_and_regenerated",
  "estate_reused_and_refreshed",
  "repaired",
  "warranty_issue",
  "issue_resolved"
]
```

This endpoint retrieves all Action Stamps.

### HTTP Request

`GET http://localhost:3000/api/v7/meta/stamps`
