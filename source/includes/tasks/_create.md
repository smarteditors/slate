## Create A Task

```ruby
example_params = {
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

> Example response

```json
{
  "status": "ok"
}
```

This endpoint creates a new Task.

### HTTP Request

`POST http://localhost:3000/api/v6/tasks`