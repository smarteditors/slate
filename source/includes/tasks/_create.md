## Create A Task

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

This endpoint creates a new Task.

### HTTP Request

`POST https://smartedi2.smarteditors.co.uk/api/v7/tasks`