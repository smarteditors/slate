## Update A Task

```ruby
example_params = {
  task: {
    location_id: String,
    description: Text,
    scheduled_date: Date,
    due_date: Date,
    assigned_to_id: String,
    assigned_by_id: String,
    reviewer_id: String
  }
}

api = EDi::APIClient
api.tasks.post(params)
```

> Example response

```json
{
  "status": "ok"
}
```

This endpoint updates a specific Task.

### HTTP Request

`PUT https://smartedi2.smarteditors.co.uk/api/v7/tasks/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The uuid of the task to update
