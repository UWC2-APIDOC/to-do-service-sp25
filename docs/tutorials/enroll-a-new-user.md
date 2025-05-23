---
layout: page
---

# Tutorial: Add a new user

This tutorial teaches you how to enroll a new user into the service. The process takes about 20 minutes to complete. Allow a total of 40 minutes if you haven't already completed "Before you start" in the following section.

## Before you start

If you haven't already, follow the instructions in [Before you start a tutorial](../before-you-start-a-tutorial.md). That topic shows you how to set up your development environment so you can use any to-do service API.

## Add a new user

In this section, you'll add a new user to the to-do service. You'll use the `POST` method to store the details of a new [`user`](../api/user.md) resource in the service. Finally, you'll observe the response to see if it looks right.

**To add a new user:**

1. Change to the `to-do-service/api` directory in your GitHub work area on your local machine and start `json-server` if it's not already running.

   ```shell
   cd <your-github-workspace>/to-do-service/api
   json-server -w to-do-db-source.json
   ```

1. Open the Postman app on your desktop and perform the following steps using it.
1. For the request method, choose POST.
1. For the URL, enter `{base_url}/users` Note: The default `{base_url}` is `http://localhost:3000/`.
1. Select the **Headers** tab.
1. Under **Key**, choose **Content-Type**.
1. Under **Value**, choose **application/json**.
1. Select the **Body** tab on the same menu bar.
1. Under that, choose **Raw**.
1. In the body, enter the `last_name`, `first_name`, and `email` as shown in the following example. Replace the values for each property with your own.

   ```js
   {
       "last_name": "Warner",
       "first_name": "Laverne",
       "email": "laverne@example.com"
    }
   ```

1. Click `Send`.

You should see a response in the bottom panel. The example response looks like this:

```js
{
    "last_name": "Warner",
    "first_name": "Laverne",
    "email": "laverne@example.com"
    "id": 6
}
```

Notice that the to-do service added a unique ID to the new user.

## Troubleshooting issues

If you see errors or no response, double-check that you have filled all the fields in correctly.

Note that there are two panels in the main window of Postman: one on top where you write the JSON to add your new user, and one below where the response appears.

## Next steps

* Learn how to [add a task](../tutorials/add-a-new-task.md) for your new user.
* Read the [`task`](../api/task.md) API reference topic.
