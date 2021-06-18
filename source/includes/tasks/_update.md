## Update A Task

```ruby
params = {
  task: {
    location_id: Integer,
    description: Text,
    scheduled_date: Date,
    due_date: Date,
    assigned_to_id: Integer,
    assigned_by_id: Integer,
    reviewer_id: Integer
  }
}

api = EDi::APIClient
api.tasks.post(params)
```

> The above command returns JSON structured like this:

```json
{
  "status": "ok"
}
```

This endpoint updates a specific Task.

### HTTP Request

`PUT http://localhost:3000/api/v6/tasks/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the task to update
