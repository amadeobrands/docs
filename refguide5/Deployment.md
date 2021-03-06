---
title: "Deployment"
category: "refguide5"
space: "Reference Guide 5"
---


A Mendix application can be deployed in different ways. You can deploy to your local machine for development and testing, you can deploy to the Mendix cloud, and you can deploy to a server you configured yourself.

## Local

You can just click "Run" in the toolbar (or use F5) to run your app locally. Use the "Open browser" button to directly jump to your app running at localhost.

If you plan to deploy to the Mendix 3.0 cloud later on and your project contains Java actions, you should enable the "Emulate Cloud Security" setting. See [Java in the Cloud](Java+in+the+Cloud) for more information.

## Mendix 5.0 Cloud

From within the Business Modeler you can view the cloud slots you have available in the Mendix Cloud. You can upload a deployment archive (mda) to the [Cloud Portal](https://cloud.mendix.com) and from there you can transfer it and start running it. See the documentation on [security constraints](Security+constraints+in+the+Mendix+Cloud) or the  section for more information.

## On-premise

Visit the [Mendix on Windows](/howto50/Deploying+Mendix+on+Microsoft+Windows), [Mendix on GNU/Linux](/howto50/Installing+Mendix+on+Debian+GNU+Linux) and [Installing Mendix on RedHat and CentOS](/howto50/Installing+Mendix+on+RedHat+and+CentOS) sections to learn how to deploy your Mendix application to servers running on these platforms.