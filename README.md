# lambda_function

# Create a Lambda Function

Navigate to the Lambda Service:

In the AWS Management Console, find the search bar at the top of the page.

Type Lambda and click on the Lambda service in the dropdown list.

Create a Function:

Click on the Create function button on the Lambda dashboard.

Select Author from scratch.

Configure the Function:

Function name: Enter a name for your Lambda function (e.g., MyTestFunction).

Runtime: Choose a programming language (e.g., Python 3.x).

Permissions: Under Permissions, select Create a new role with basic Lambda permissions.

Click on the Create function button at the bottom.

Step 1: Add Code to Your Lambda Function

Edit the Function Code:

After your function is created, you will see the code editor.

In the code editor, replace any existing code with the following simple handler:

def lambda_handler(event, context):
    return {
        'statusCode': 200,
        'body': 'Hello from Lambda!'
    }


Deploy Your Changes:

Click the Deploy button in the top right corner to save your changes.
Step 2: Test Your Lambda Function

Create a Test Event:

Click on the Test button located in the top right corner of the Lambda console.

In the pop-up window, name your test event (e.g., TestEvent).

You can leave the default settings as they are.

Click on Create.

Run the Test:

After creating the test event, click the Test button again.

The Lambda console will execute your function, and you will see the results in the Execution results section below.

If successful, you should see output similar to:

{
    "statusCode": 200,
    "body": "Hello from Lambda!"
}
