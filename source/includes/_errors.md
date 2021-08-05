# Errors

> Some `4xx` errors that could be handled programmatically (e.g., an asset wasn't found) include an error code that briefly explains the error reported.

```json
{
  "request_id": "c9f7d475-9252-46e5-ba3d-c97fee579098",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "message": "Invalid attributes, validation failed.",
  "errors": [
    "Location must exist",
    "Condition can't be blank",
    "Status can't be blank",
    "Code has already been taken"
  ]
}
```

SmartED-i API uses conventional HTTP response codes to indicate the success or failure of an API request. 
- Codes in the `2xx` range indicate success. 
- Codes in the `4xx` range indicate an error that failed given the information provided (e.g., a required parameter was omitted, an asset update failed, etc.). 
- Codes in the `5xx` range indicate an error with SmartED-i's servers (however these are extremely rare).


<!-- 
# Errors

<aside class="notice">
This error section is stored in a separate file in <code>includes/_errors.md</code>. Slate allows you to optionally separate out your docs into many files...just save them to the <code>includes</code> folder and add them to the top of your <code>index.md</code>'s frontmatter. Files are included in the order listed.
</aside>

The Kittn API uses the following error codes:


Error Code | Meaning
---------- | -------
400 | Bad Request -- Your request is invalid.
401 | Unauthorized -- Your API key is wrong.
403 | Forbidden -- The kitten requested is hidden for administrators only.
404 | Not Found -- The specified kitten could not be found.
405 | Method Not Allowed -- You tried to access a kitten with an invalid method.
406 | Not Acceptable -- You requested a format that isn't json.
410 | Gone -- The kitten requested has been removed from our servers.
418 | I'm a teapot.
429 | Too Many Requests -- You're requesting too many kittens! Slow down!
500 | Internal Server Error -- We had a problem with our server. Try again later.
503 | Service Unavailable -- We're temporarily offline for maintenance. Please try again later. -->
