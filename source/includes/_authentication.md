# Authentication

The SmartED-i API uses API keys to authenticate requests. You can view and manage your API keys in your SmartED-i API Dashboard.

Test mode secret keys have the prefix `sk_test_` and live mode secret keys have the prefix `sk_live_`.

Your API keys carry many privileges, so be sure to keep them secure! Do not share your secret API keys in publicly accessible areas such as GitHub, client-side code, and so forth.

> Provide your API key via the `key` header in every request.