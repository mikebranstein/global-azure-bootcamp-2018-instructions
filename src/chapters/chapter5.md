## Deploying Custom Speech Service Endpoints

In this chapter, you'll learn how to:
- deploy your customized acoustic and language models and create a secured endpoint
- test the customized CSS endpoint using the web app you deployed earlier  

### Overview

Previously, you learned about the various data sets you need to train, test, and operationalize machine learning systems. Over the past 2 chapters, you created training and testing data sets, built customized acoustic and language models, then tested the customization accuracy.

The next step is to deploy your customization and test them with real-world data.

Let's get started!

### Deploying Custom Models

You've already done the hard work of building the customized models, so let's use them to create a deployment.

> **PREREQUISITES**
>
> Before you proceed, you'll need a customized acoustic and language model that have a *Succeeded* status. If your models are still training, wait a few more minutes, then check back when the models are ready.

<h4 class="exercise-start">
    <b>Exercise</b>: Deploying customized acoustic and language models
</h4>

Start by navigating to the CSS web portal at <a href="https://cris.ai" target="_blank">https://cris.ai</a>, and navigate to *Deployments*. 

Click the *Create New* button to create a new deployment.

Complete the following fields:
- Locale: en-US
- Description: *blank*
- Name: Pokemon
- Subscription: *the one you created earlier*
- Base Model: Microsoft Search and Diction Model, then select the Pokemon models below

<img src="images/chapter5/deploy1.png" class="img-override" />

Click *Create* to deploy the models to production.

When the test run is saved, you'll navigate back to the *Deployments* page:

<img src="images/chapter5/deploy2.png" class="img-override" />

Note the *Status* of the test run is *NotStarted*. In a few moments, it will change to *Running*, then *Succeeded*.

The deployment will not take long (up to 1 minute). That's it! You've deployed your models.

This concludes the exercise. 

<div class="exercise-end"></div> 

### Testing the Custom Speech Service Endpoint

