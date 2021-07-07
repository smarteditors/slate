## Get All Tasks

```ruby
api = EDi::APIClient
api.tasks
```

> Example response

```json
[
  {
    "id": 1,
    "assigned_to_id": 2,
    "assigned_by_id": 2,
    "uuid": "87832ba2-2dda-4933-a69c-edc5889e1bed",
    "description": "here is a work request",
    "scheduled_date": "2021-06-16T00:00:00.000+01:00",
    "created_at": "2021-06-17T15:22:27.000+01:00",
    "draft": false,
    "reviewer_id": 2,
    "client_id": 1,
    "items": [
      {
        "id": 19,
        "client_id": 1,
        "condition_id": 3,
        "status_id": 23,
        "code": "0000000213",
        "usage": "in_use",
        "project": "sdd",
        "catalogue_item_id": "7e9fe938-f2db-4cd5-8259-f22db5806a9c",
        "slug": "213",
        "uuid": "70c86852-36fb-4879-88ed-ff57f29fc492",
        "created_at": "2021-05-25T16:29:14.000+01:00",
        "updated_at": "2021-06-07T11:47:44.000+01:00",
        "location_id": 8,
        "x": null,
        "y": null,
        "actions": [
          {
            "status": "created",
            "date": "2021-05-25T16:29:14.000+01:00",
            "location": "5509613e-ee0e-403e-9de9-dc9f500c3dd3"
          }
        ],
        "warranty": 15,
        "warranty_info": "vjk",
        "purchase_price_cents": 123,
        "purchase_price_currency": "£",
        "purchase_date": "2021-01-20T00:00:00.000+00:00",
        "action_id": 4,
        "action_date": "2021-06-04T00:00:00.000+01:00",
        "room": "new",
        "colour": "#000000",
        "reuse_action_id": null,
        "stamps_count": 18,
        "item_attributes_count": 0,
        "in_storage": false,
        "sale_price": 120.0,
        "installation_date": null,
        "life_expectancy": 0.0,
        "asset_type": "asset",
        "condition_details": null,
        "pre_charged_for_disposal": false,
        "photo": null,
        "condition": {
          "id": 3,
          "name": "poor",
          "label": "Poor",
          "description": null,
          "uuid": "cb274607-0af0-40a1-96c9-3324d0639982",
          "created_at": "2020-11-09T13:08:36.000+00:00",
          "updated_at": "2020-11-09T13:08:36.000+00:00",
          "client_id": null,
          "colour": null,
          "is_default": false
        },
        "status": {
          "id": 23,
          "name": "waiting_regeneration",
          "label": "Awaiting Regeneration",
          "description": null,
          "status_type": null,
          "uuid": "69bd2c6f-7311-421c-b956-4c55955ebe63",
          "created_at": "2020-11-09T13:08:36.000+00:00",
          "updated_at": "2020-11-09T13:08:36.000+00:00",
          "reportable": true,
          "reprocessable": false,
          "archivable": false,
          "icon_name": null,
          "icon_family": null,
          "icon": {
            "url": null
          },
          "width": null,
          "height": null,
          "client_id": null,
          "is_default": false,
          "reusable": false
        }
      }
    ],
    "task_items": [
      {
        "id": 1,
        "task_id": 1,
        "item_id": 19,
        "completed_by_id": null,
        "uuid": "493bd7c5-d695-40f4-932f-94ed00d31626",
        "completed": null,
        "completed_date": null,
        "created_at": "2021-06-17T15:22:27.000+01:00",
        "updated_at": "2021-06-17T15:22:27.000+01:00"
      }
    ]
  }
]
```

This endpoint retrieves all draft tasks for the current client or the assigned tasks for the current user.

### HTTP Request

`GET http://localhost:3000/api/v7/tasks`

### Query Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | -------- | -------
draft | false | If true, return draft tasks for the current client | boolean | false

??? calls client.tasks, but no tasks association/method on client, so :draft doesn't work