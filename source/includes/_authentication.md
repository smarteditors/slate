# Authentication

??? This isn't exactly right i don't think? we have an authenticate end point that takes an email and password, then you have to submit a 'token' in the header (not 'key') 

The SmartED-i API uses API keys to authenticate requests. You can view and manage your API keys in your SmartED-i API Dashboard.

Test mode secret keys have the prefix `sk_test_` and live mode secret keys have the prefix `sk_live_`.

Your API keys carry many privileges, so be sure to keep them secure! Do not share your secret API keys in publicly accessible areas such as GitHub, client-side code, and so forth.

> Provide your API key via the `key` header in every request.