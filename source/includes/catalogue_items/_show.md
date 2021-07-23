## Get a Specific Catalogue Item

> `GET http://localhost:3001/api/v6/items/d55010cb-5d05-4749-b6b4-f08070cc21bb`

> Example response

```json
{
  "request_id": "4e69141c-cb46-4687-9fc1-3bdb08b8698e",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "item": {
    "uuid": "e4f05457-9153-435d-9502-04cb7f8ba0ea",
    "archived": false,
    "catalogue": {
      "uuid": "91eef228-5a8d-4eb5-9a44-22af1c6307d0",
      "name": "dvzdv"
    },
    "category": {
      "uuid": "d55010cb-5d05-4749-b6b4-f08070cc21bb",
      "archived": false,
      "catalogue_id": "91eef228-5a8d-4eb5-9a44-22af1c6307d0",
      "client_id": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
      "colour": "#000000",
      "depreciation_rate": 1.0,
      "depreciation_term": 0,
      "icon_content_type": null,
      "icon_file_size": null,
      "icon_updated_at": null,
      "name": "test category",
      "slug": null
    },
    "client_id": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
    "code": "sacsa",
    "components": [],
    "confirmed": true,
    "csr_confirmation": false,
    "cubic": 3.0,
    "cubic_size": 3.0,
    "depreciation_rate": 0.1,
    "depreciation_term": 0,
    "description": "",
    "display_status": "Awaiting Decision",
    "embedded_co2": null,
    "from_edi": false,
    "house_position": "",
    "locking_user_id": null,
    "locking_user_name": null,
    "material": "",
    "max_stock_level": -1,
    "min_stock_level": -1,
    "name": "a style",
    "photo": "/images/missing.jpg",
    "photo_content_type": null,
    "photo_file_name": null,
    "photo_file_size": null,
    "photo_updated_at": null,
    "price_as_new": null,
    "rate": 0.1,
    "sale_or_donation": "",
    "sales_reference": "S000002",
    "sfg": "sacsa",
    "slug": null,
    "snd_max_price": null,
    "snd_min_price": null,
    "status": "awaiting_decision",
    "status_locked": false,
    "status_locked_at": null,
    "status_unlocked_at": null,
    "supplier_id": null,
    "term": 0,
    "type": {
      "uuid": "574fbbc9-fcea-4dd4-b1df-7e6f9c2ccdf4",
      "archived": false,
      "category_id": "d55010cb-5d05-4749-b6b4-f08070cc21bb",
      "client_id": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
      "cubic_size": 3.0,
      "depreciation_rate": 1.0,
      "depreciation_term": 0,
      "icon_content_type": null,
      "icon_file_name": null,
      "icon_file_size": null,
      "icon_updated_at": null,
      "name": "chair",
      "slug": null
    },
    "used_for": [],
    "weight": null
  },
  "attribute_associations": []
}
```

This endpoint retrieves a specific Item.

### HTTP Request

`GET http://localhost:3001/api/v6/items/<ID>`
