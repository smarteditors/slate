---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - ruby

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/slatedocs/slate'>Documentation Powered by Slate</a>

includes:
  - actions/header
  - actions/index
  - actions/show

  - clients/header
  - clients/index
  - clients/show
  - clients/set_current_client

  - conditions/header
  - conditions/index
  - conditions/show

  - items/header
  - items/index
  - items/show
  - items/create
  - items/update
  - items/validate_code

  - locations/header
  - locations/index
  - locations/show
  - locations/population
  - locations/search

  - photos/header
  - photos/create
  - photos/update

  - sessions/header
  - sessions/client
  - sessions/user
  - sessions/logout

  - stamps/header
  - stamps/index

  - statuses/header
  - statuses/index
  - statuses/show

  - store_me_groups/header
  - store_me_groups/index
  - store_me_groups/show

  - tasks/header
  - tasks/index
  - tasks/show
  - tasks/create
  - tasks/update

  - users/header
  - users/index

  - errors

search: true

code_clipboard: true
---

# Introduction

Welcome to the Kittn API! You can use our API to access Kittn API endpoints, which can get information on various cats, kittens, and breeds in our database.

We have language bindings in Shell, Ruby, Python, and JavaScript! You can view code examples in the dark area to the right, and you can switch the programming language of the examples with the tabs in the top right.

This example API documentation page was created with [Slate](https://github.com/slatedocs/slate). Feel free to edit it and use it as a base for your own API's documentation.

# Authentication

> To authorize, use this code:

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
```

```shell
# With shell, you can just pass the correct header with each request
curl "api_endpoint_here" \
  -H "Authorization: meowmeowmeow"
```

```javascript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
```

> Make sure to replace `meowmeowmeow` with your API key.

Kittn uses API keys to allow access to the API. You can register a new Kittn API key at our [developer portal](http://example.com/developers).

Kittn expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: meowmeowmeow`

<aside class="notice">
You must replace <code>meowmeowmeow</code> with your personal API key.
</aside>

