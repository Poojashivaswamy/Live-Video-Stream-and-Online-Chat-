# Amazon IVS Simple Chat demo

A demo web application intended as an educational tool for demonstrating how you can build a very simple Chat backend. In conjunction with Amazon IVS, it can be used to build a compelling customer experience for live streams with chat use-cases.

<img src="simple-chat-demo.png" alt="Amazon IVS Simple Chat demo" />


This is a serverless web application, leveraging [Amazon IVS](https://aws.amazon.com/ivs/), [AWS Lambda](https://aws.amazon.com/lambda/), and WebSockets. The web user interface is a [single page application](https://en.wikipedia.org/wiki/Single-page_application) built using [responsive web design](https://en.wikipedia.org/wiki/Responsive_web_design) frameworks and techniques, producing a native app-like experience tailored to the user's device.


The demo showcases how you can implement a simple chat client next to an Amazon IVS stream. Users are asked to enter their name the first time they begin chatting. Messages are sent in the format `<Username>` `<Message>` as part of each chat "bubble". Users can send plain text messages, text links, and emojis. Chat messages have a character limit of 510 characters.

## Getting Started

***IMPORTANT NOTE:** Deploying this demo application in your AWS account will create and consume AWS resources, which will cost money.*

This demo is comprised of two parts: `serverless` (the demo backend) and `web-ui` (the demo frontend).

1. If you do not have an AWS account, please see [How do I create and activate a new Amazon Web Services account?](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)
2. Log into the [AWS console](https://console.aws.amazon.com/) if you are not already. Note: If you are logged in as an IAM user, ensure your account has permissions to create and manage the necessary resources and components for this application.
3. [Test locally or deploy](./serverless/README.md) to your AWS account.

## Known issues and limitations
* The application was written for demonstration purposes and not for production use.
* Currently only tested in the us-west-2 (Oregon) region. Additional regions may be supported depending on service availability.

## About Amazon IVS
Amazon Interactive Video Service (Amazon IVS) is a managed live streaming solution that is quick and easy to set up, and ideal for creating interactive video experiences. [Learn more](https://aws.amazon.com/ivs/).

* [Amazon IVS docs](https://docs.aws.amazon.com/ivs/)
* [User Guide](https://docs.aws.amazon.com/ivs/latest/userguide/)
* [API Reference](https://docs.aws.amazon.com/ivs/latest/APIReference/)
* [Setting Up for Streaming with Amazon Interactive Video Service](https://aws.amazon.com/blogs/media/setting-up-for-streaming-with-amazon-ivs/)
