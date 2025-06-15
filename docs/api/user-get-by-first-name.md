---
layout: page
---

# Get user by first name

Returns an array of [user](user.md) objects that contain only the user specified by the `first_name` parameter, if it exists.

## URL

```shell

{server_url}/users/{first_name}
```

## Parameters

| Parameter name | Type | Description |
| -------------- | ------ | ------------ |
| `first_name` | string | The first name of the user to return |

## Request headers

None

## Request body

None

## Return body

```json
[
    {
        "last_name": "Smith",
        "first_name": "Ferdinand",
        "email": "f.smith@example.com",
        "id": 2
    }
]
```

## Return status

| Status value | Return status | Description |
| ------------- | ----------- | ----------- |
| 200 | Success | Requested data returned successfully |
| 404 | Error | Specified user record not found |
|  ECONNREFUSED | N/A | Service is offline. Start the service and try again. |

## Related read operations

* [Get all users](users-get-all-users.md)
* [Get users by ID](users-get-user-by-id.md)
