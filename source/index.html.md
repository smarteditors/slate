---
title: API Reference

# language_tabs: # must be one of https://git.io/vQNgJ
#   - ruby

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/slatedocs/slate'>Documentation Powered by Slate</a>

includes:
  - authorisation/authorisation

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

  - errors

search: true

code_clipboard: true
---

# Introduction

The SmartED-i API is organised around REST. Our API has predictable resource-oriented URLs, accepts and returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.

You can use the SmartED-i API in test mode, which does not affect your live data. The API key you use to authenticate the request determines whether the request is live mode or test mode.

The SmartED-i API differs for every account as we release new versions and tailor functionality.

