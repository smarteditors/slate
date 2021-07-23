---
title: SmartED-i API Reference

# language_tabs: # must be one of https://git.io/vQNgJ
#   - ruby

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/slatedocs/slate'>Documentation Powered by Slate</a>

includes:
  - authorisation/authorisation
  - errors

  - sessions/header
  - sessions/authenticate
  - sessions/client
  - sessions/user
  - sessions/logout

  # - actions/header
  # - actions/index
  # - actions/show

  - clients/header
  - clients/index
  - clients/show
  - clients/set_current_client

  - conditions/header
  - conditions/index
  # - conditions/show

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
  # - locations/search

  - photos/header
  - photos/create
  - photos/update

  # - stamps/header
  # - stamps/index

  - statuses/header
  - statuses/index
  # - statuses/show

  # - store_me_groups/header
  # - store_me_groups/index
  # - store_me_groups/show

  # - tasks/header
  # - tasks/index
  # - tasks/show
  # - tasks/create
  # - tasks/update

  - users/header
  - users/index


  # catalogue api
  - asset_attributes/header
  - asset_attributes/index

  - attribute_associations/header
  - attribute_associations/index

  - attributes/header
  - attributes/index

  - catalogue_items/header
  - catalogue_items/index
  - catalogue_items/show
  - catalogue_items/search
  - catalogue_items/filter
  - catalogue_items/code_search
  - catalogue_items/check_code
  # - catalogue_items/create

  - catalogue_photos/header
  - catalogue_photos/update

  - catalogues/header
  - catalogues/index
  - catalogues/show

  - categories/header
  - categories/index
  - categories/show
  - categories/search

  - colour_board_colours/header
  - colour_board_colours/index
  
  - types/header
  - types/index
  - types/show

search: true

code_clipboard: true
---

# Introduction

The SmartED-i API is organised around REST. Our API has predictable resource-oriented URLs, accepts and returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.

You can use the SmartED-i API in test mode, which does not affect your live data. The API key you use to authenticate the request determines whether the request is live mode or test mode.

The SmartED-i API differs for every account as we release new versions and tailor functionality.


# Authentication

The SmartED-i API uses API keys to authenticate requests. You can view and manage your API keys in your SmartED-i API Dashboard.

Test mode secret keys have the prefix `sk_test_` and live mode secret keys have the prefix `sk_live_`.

Your API keys carry many privileges, so be sure to keep them secure! Do not share your secret API keys in publicly accessible areas such as GitHub, client-side code, and so forth.

> Provide your API key via the `key` header in every request.