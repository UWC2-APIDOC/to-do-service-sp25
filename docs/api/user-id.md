---
layout: page
---

# `PUT /users/{userId}` 

This API updates existing user Idd. If a user Id has not been created, you can use this API to create one.

## URL

```shell
{server_url}/users/{userId} 
```

## Parameters

```http
None
```

## Headers

```http
USER.ID
required
string <uuid> = 36 characters
Specifies the value for <consumer_id>.

This is the User ID value for the OAuth2 authentication, which will be provided by the client's Technical Account Manager

Example: 685f74bf-b8ca-447d-8338-966di751443f
```

## Request

```http
{
"users": {
"userId": "4969",
{
}
```

## Response

```shell
'200':
description: OK. The request was successful, and the server returned the requested data. No response object is returned.

{
"isEligibleUserId": true,
{
"userId": "4969"
}
```

