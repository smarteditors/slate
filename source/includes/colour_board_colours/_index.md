## Get A List Of Colour Board Colours

> `GET http://localhost:3001/api/v6/colour_board_colours`

> Example response

```json
{
  "request_id": "4d578828-94e7-402b-b584-682eb4e2c2d5",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "colours": [
    {
      "uuid": "21c03cc0-5d19-48c1-b346-a0e2fd4114cd",
      "colour_type": null,
      "name": "test colour",
      "value": null
    }
  ]
}
```

This endpoint retrieves a list of Colour Board Colours for the current client or for a specified Colour Board, Category, or by a list of uuids. 

??? array passing is weird. need to change or explain how to do it

### HTTP Request

`GET http://localhost:3001/api/v6/categories`


### Query Parameters

Parameter | Default | Description | Type | Required?
--------- | ------- | ----------- | ---- | --------
colour_board_id | nil | The uuid of a Colour Board | String | No
category_id | nil | The uuid of a Category | String | No
colour_ids | nil | The uuids of ColourBoardColours | String | No