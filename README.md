# TaskMasterAPI

## These are Steps for the week.

URL for frontend:
http://elasticbeanstalk-us-west-2-074808275502.s3-website-us-west-2.amazonaws.com/


### Testing:
Please use postman for all test.

### Feature 1:
I created a create method to My API gateway while using a Lambda funtion.
To create a task you can use the following URL: 
Post:
https://8o88ocps78.execute-api.us-west-2.amazonaws.com/dev/tasks
The task has to be posted in Json format.

### Example 
{
"assignee": "Fabian",
"title":"Writing example",
"description": "making an example for a task post method"
}

### Feature 2:
I created a method to get all the task that have been created.
Use the following URL:
Get:
https://8o88ocps78.execute-api.us-west-2.amazonaws.com/dev/tasks

### Feature 3:
I created a method to get all the tesk assigned to a certain person:
Use the following URL:
Get:
https://8o88ocps78.execute-api.us-west-2.amazonaws.com/dev/tasks/assignee/{assignee}

### Example
https://8o88ocps78.execute-api.us-west-2.amazonaws.com/dev/tasks/assignee/Fabian

### Feature 4: 
I created a method to checng the state/status of the task.
Use the following URL:
https://8o88ocps78.execute-api.us-west-2.amazonaws.com/dev/tasks/state/{id}

### Example
https://8o88ocps78.execute-api.us-west-2.amazonaws.com/dev/tasks/state/48b4e468-1bb5-485b-ad59-f348844094ff

### Feature 5:
I created a method to delete a task that was created.
Use the following URL:
https://8o88ocps78.execute-api.us-west-2.amazonaws.com/dev/tasks/{id}

### Example
https://8o88ocps78.execute-api.us-west-2.amazonaws.com/dev/tasks/48b4e468-1bb5-485b-ad59-f348844094ff

# Contributors

Kevin Couture,
Nicholas Paro,
Padmapriya Ganapathi,
Jack Kinne

# Resources
I use an AWS Lambda github to find out about APIProxyRequestEvent and APIProxyResponse.

### Response: 
https://github.com/aws/aws-lambda-java-libs/blob/master/aws-lambda-java-events/src/main/java/com/amazonaws/services/lambda/runtime/events/APIGatewayProxyResponseEvent.java

### Request: 
https://github.com/aws/aws-lambda-java-libs/blob/master/aws-lambda-java-events/src/main/java/com/amazonaws/services/lambda/runtime/events/APIGatewayProxyResponseEvent.java




