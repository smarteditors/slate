## Update A Photo

> `PUT http://localhost:3000/api/v6/photos/73f5f971-c6d6-4495-b2bf-022380d27c23`

```ruby
example_params = {
  file: [String]
}
```

> Example response

```json
{
  "item": {
    "id": 28,
    "item_id": "56d844f6-ebdf-476e-932b-8b7ca565b77e",
    "image": {
      "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/photo/image/28/hancock.jpeg",
      "thumb": {
        "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/photo/image/28/thumb_hancock.jpeg"
      },
      "large": {
        "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/photo/image/28/large_hancock.jpeg"
      },
      "square": {
        "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/photo/image/28/square_hancock.jpeg"
      },
      "portrait": {
        "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/photo/image/28/portrait_hancock.jpeg"
      }
    },
    "width": null,
    "height": null,
    "uuid": "ab0c490d-93aa-4ba0-beae-58d160ad0132",
    "created_at": "2021-06-09T14:10:03.000+01:00",
    "updated_at": "2021-06-28T12:39:50.000+01:00",
    "image_source_url": null,
    "image_file_name": null,
    "image_tmp": null
  },
  "status": "updated"
}
```

This endpoint attached a file to a specific Photo record.

### HTTP Request

`PUT http://localhost:3000/api/v6/photos/<ID>`


### URL Parameters

Parameter | Description
--------- | -----------
ID | The uuid of the Photo to update


### Supported Media Types

multipart/form-data

### Params

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
file | nil | A file upload | String | Yes |