## Publishing and Testing LUIS Apps

In this chapter, you'll learn how to:
- train your LUIS app
- test a trained app
- publish a trained LUIS app

### Overview

The concept of training a LUIS app is like training Custom Speech Service apps. So far, you've created a training data set including intents and entities, so the next step is to train your app. Then you'll test the trained app, and publish for consumption.

In a real-world scenario, you'll incrementally advance the functionality of a LUIS app. For example, you'll start with a few intents and entities, then as your app matures (or when you identify a deficiency), you'll add new intents and entities, re-train, and publish a new version of the LUIS app.

Let's jump into the training process.

### Training LUIS

Training a LUIS app is easy. Seriously. I don't like to refer to machine learning concepts as *easy*, but all you do is click a button. 

<h4 class="exercise-start">
    <b>Exercise</b>: Training your LUIS app 
</h4>

Log in to the LUIS portal at [https://luis.ai](https://luis.ai), and navigate to the *My Apps* areas, drilling down into the *Pokemon* app.

In the upper-right corner, you'll see a *Train* button. Visually, the button will appear with a red dot when there are changes in the LUIS app that can be trained. Hovering over the button also indicates that it can untrained changes.

Click the *Train* button to train your LUIS app, integrating intents and entities into the trained app model:

<img src="images/chapter8/training.gif" class="img-override" />

When training is finished, the *Train* button has a green dot:

<img src="images/chapter8/train1.png" class="img-override" />

That's it. It was easy.

This concludes the exercise. 

<div class="exercise-end"></div>

### Testing LUIS

Now that your LUIS app is trained, you can test it. The LUIS portal offers a cool testing utility embedded, so it makes testing your app quick.

Let's test a few phrases that we may expect our app should handle.

<h4 class="exercise-start">
    <b>Exercise</b>: Testing your LUIS app 
</h4>

Log in to the LUIS portal at [https://luis.ai](https://luis.ai), and navigate to the *My Apps* areas, drilling down into the *Pokemon* app.

In the upper-right corner, you'll see a *Test* button. 

<img src="images/chapter8/test1.png" class="img-override" />

Click the *Test* button and a sidebar will pop out. In the textbox, enter in several utterances and see how your trained LUIS app performs. 

Try these utterances:
- Pikachu sit down.
- Jigglypuff jump.
- Stop being so loud Jigglypuff.

<img src="images/chapter8/test.gif" class="img-override" />

That's it for testing in the LUIS portal. 

This concludes the exercise. 

<div class="exercise-end"></div>

With a tested LUIS app that you're satisfied with, let's move on to publishing your LUIS app.

### Publishing a LUIS App

