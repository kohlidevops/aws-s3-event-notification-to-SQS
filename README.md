# aws-s3-event-notification-to-SQS

**To Configure Event notification with SQS and Polling message from SQS Queue**

**To Create a S3 bucket**

<img width="611" alt="image" src="https://github.com/kohlidevops/aws-s3-event-notification-to-SQS/assets/100069489/67793c3b-6084-4777-8e12-1ff8649c8175">

**To Create a SQS Queue**

I'm going to create a SQS Queue with standard method and others are leave as default.

<img width="668" alt="image" src="https://github.com/kohlidevops/aws-s3-event-notification-to-SQS/assets/100069489/f659d6f4-bd3f-4a71-b7c5-cef9455de14d">

**To configure Resource Access Policy in SQS**

To configure the SQS Resource Access Policy to accept the event notification from S3 bucket. To edit the Resource Access Policy - Select - Policy generator - create a policy. Below link to use Resource Access Policy

**https://github.com/kohlidevops/aws-s3-event-notification-to-SQS/blob/main/sqs-resource-access-policy**

**Configure Event Notification**

To select your S3 bucket - Properties - Create Event Notification with All Object create event

<img width="761" alt="image" src="https://github.com/kohlidevops/aws-s3-event-notification-to-SQS/assets/100069489/fdccdcc3-4804-4154-b70d-45403a713813">

Destination - Select - your SQS and save the Event Notification

<img width="725" alt="image" src="https://github.com/kohlidevops/aws-s3-event-notification-to-SQS/assets/100069489/cda5d0e8-0be9-4af3-8885-dbab36038df5">

**Upload objects**

To upload some object to s3 bucket and back to SQS Queue - select - your SQS Queue - choose - Send and recieve messages - hit - Poll for messages

After Polling you can see message in SQS which containes S3 object key, size, event type and so on.

That's it.










