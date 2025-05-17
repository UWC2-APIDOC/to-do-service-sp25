# Tutorial: Delete a User
In this tutorial, you learn the operations to call to delete a user from the service. Expect this tutorial to take about 15 minutes to complete.

## Before You Start
Make sure you've completed the "Before you start a tutorial" topic on the development system you'll use for the tutorial.

## Delete a User
Deleting a user from the service requires that you use the DELETE method to remove the user resource from the service.

#### To delete a user:

1. Make sure your local service is running, or start it by using this command, if it's not:
cd <your-github-workspace>/to-do-service/api json-server -w to-do-db-source.json
2. Open the Postman app on your desktop.
3. In the Postman app, create a new request with these values:
- METHOD: DELETE
- URL: {{base_url}}/users/{userId} (replace {userId} with the actual ID of the user you want to delete)
- Headers: Content-Type: application/json
4. In the Postman app, choose **Send** to make the request.
5. Watch for the response body, which should confirm the deletion of the user.
  
After doing this tutorial in Postman, you might like to repeat it in your favorite programming language. To do this, adapt the values from the tutorial to the properties and arguments that the language uses to make REST API calls.
