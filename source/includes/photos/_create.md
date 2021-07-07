## Create A Photo

> `POST http://localhost:3000/api/v7/photos`

```ruby
example_params = {
  photo: {
    uuid: String,
    item_id: Integer,
    image_source_url: String,
    created_at: DateTime
  }
}
```

> Example response

```json
{
  "request_id": "ee821c97-c29c-496f-aa5f-43c37f3493a0",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "photo": {
    "uuid": "62d2791a-ca8b-4248-907c-7cc288c590a7",
    "height": null,
    "image": {
      "url": null,
      "thumb": {
        "url": null
      },
      "large": {
        "url": null
      },
      "square": {
        "url": null
      },
      "portrait": {
        "url": null
      }
    },
    "image_file_name": null,
    "image_source_url": null,
    "image_tmp": null,
    "item_id": null,
    "width": null
  }
}
```

This endpoint creates a new Photo record linked to an item. If the uuid of an existing record is submitted that record is updated instead of a new record being created. This endpoint does not allow the uploading of photo files. after the photo record is created, the photo file for the record is uploaded via the photos/update endpoint.


### HTTP Request

`POST http://localhost:3000/api/v7/photos`


### Photo Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
uuid | nil | The uuid of the photo to be created or updated | String | No
item_id | nil | The uuid of the item the photo is attached to | Integer | Yes