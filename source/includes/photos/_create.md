## Create A Photo

> `POST http://localhost:3000/api/v6/photos`

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
  "item": {
    "id": 30,
    "item_id": "22",
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
    "width": null,
    "height": null,
    "uuid": "73f5f971-c6d6-4495-b2bf-022380d27c23",
    "created_at": "2021-06-18T10:09:05.000+01:00",
    "updated_at": "2021-06-18T10:09:05.000+01:00",
    "image_source_url": "https://i.kym-cdn.com/entries/icons/facebook/000/006/360/gottago.jpg",
    "image_file_name": null,
    "image_tmp": null
  },
  "status": "created"
}
```

This endpoint creates a new Photo record linked to an item. If the uuid of an existing record is submitted that record is updated instead of a new record being created. This endpoint does not allow the uploading of photo files. after the photo record is created, the photo file for the record is uploaded via the photos/update endpoint.


### HTTP Request

`POST http://localhost:3000/api/v6/photos`


### Photo Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
uuid | nil | The uuid of the photo to be created or updated | String | No
item_id | nil | The uuid of the item the photo is attached to | Integer | Yes