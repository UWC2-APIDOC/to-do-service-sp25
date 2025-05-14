# To-do service overview

Use the To-Do Service to post common tasks and recieve reminders for those tasks.

## Get started

Before you can begin to perform common tasks with the **To-Do service**, you must set up your development system. Review the [Before you start a tutorial](https://uwc2-apidoc.github.io/to-do-service-sp25/before-you-start-a-tutorial/) page to get started.
>[!NOTE]
>Preparation to start a tutorial takes approximately 20 minutes to complete.

## Order of tasks

To begin posting your tasks to the service, you must add your users to the service first.

1. [Enroll a new user](https://uwc2-apidoc.github.io/to-do-service-sp25/tutorials/enroll-a-new-user/)
2. [Add a new task](https://uwc2-apidoc.github.io/to-do-service-sp25/tutorials/add-a-new-task/)

## Coming soon

The following tasks for the **To-Do service** are available soon:

- Change the due-date of a task
- Delete a task
- Get all tasks
- Get task by ```ID```
- Get task by ```user_ID```

## References by resource

### User resource

The [user resource](https://uwc2-apidoc.github.io/to-do-service-sp25/api/user/) contains information for all users of the service.

The following is an example of the user resource:

```json
{
    "last_name": "Smith",
    "first_name": "Ferdinand",
    "email": "f.smith@example.com",
    "id": 1
}
```

### Task resource

The [task resource](https://uwc2-apidoc.github.io/to-do-service-sp25/api/task/) contains information for all tasks in the service.

The following is an example of the task resource:

```json
{
    "user_id": 1,
    "title": "Grocery shopping",
    "description": "eggs, bacon, gummy bears",
    "due_date": "2025-02-20T17:00",
    "warning": "-10",
    "id": 1
}
```
