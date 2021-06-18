## Create A Photo

```ruby
params = {
  photo: {
    uuid: String, ???
    item_id: Integer,
    image_source_url: String
  }
}

api = EDi::APIClient
api.photos.post(params)
```

> The above command returns JSON structured like this:

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

This endpoint creates a new Photo linked to an item.

### HTTP Request

`POST http://localhost:3000/api/v6/photos`
