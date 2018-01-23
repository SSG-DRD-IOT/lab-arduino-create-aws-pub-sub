[AWS Alliance Workshop](https://github.com/SSG-DRD-IOT/Alliance-AWS-Workshop) > [Arduino Create AWS PubSub Lab](lab-arduino-create-aws-pub-sub.md)

# Arduino Create - AWS Pub/Sub Lab

This lab will walk you through setting up a basic data connection between your UP2 Board and AWS IoT using Arduino Create. 

### Prerequisites
You will need to have completed the following steps:
*	Setup UP2 board
*	Connect UP2 board to Arduino Create 
*	Complete the [Sensors and Actuators](https://ssg-drd-iot.github.io/toc-sensors)
* Complete the [AWS IoT Setup](https://ssg-drd-iot.github.io/lab-aws-iot)

## Load Pub/Sub Example 

Arduino Create has the AWS IoT Device SDK buit in. You will use this SDK to connect your UP2 board to AWS IoT. We will be editing the Pub/Sub example.

Load the example through Examples -> From Libraries -> AWS IoT Device SDK -> PubSub
![](./images/pubsub-example.png)

## Configure Pub/Sub Example

You will need to change the **ENDPOINT, CLIENT_ID, and THING_NAME** on lines 43-45 to those given to you by AWS IoT. To find the **ENDPOINT** navigate to the AWS Console -> AWS IoT -> Manage -> Things 

![](./images/aws-things.png)

Select the Thing that you configured and naviagte to **Interact**. The rest API endpoint is the **ENDPOINT** you will use. 

![](./images/aws-things-interact.png)
