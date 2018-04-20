## Building a LUIS App

In this chapter, you'll learn:
- how to build intents
- how to create entities and map them to intent phrases
- how to improve accuracy of LUIS using phrase lists

### Overview

In the last chapter you learned about the basics of LUIS: intents, utterances, entities. You also learned how we'll be using LUIS and how it will integrate into our speech-to-text pipeline.

I don't want to delay us too much, so let's dive right in by creating your first LUIS app.

### Creating a LUIS app

<h4 class="exercise-start">
    <b>Exercise</b>: Creating a LUIS App
</h4>

Log in to the LUIS portal at [https://luis.ai](https://luis.ai), and navigate to the *My Apps* area:

<img src="images/chapter7/luis1.png" class="img-override" />

This page lists the various LUIS apps you have created.

Click the *Create new app* button. Name it *Pokemon*:

<img src="images/chapter7/luis2.png" class="img-override" />

After creating the app, you be redirected to the *Intent* page automatically:

<img src="images/chapter7/luis3.png" class="img-override" />

There's not much more to creating the initial LUIS app, so let's continue on with defining your app intents.

This concludes the exercise. 

<div class="exercise-end"></div>

### Creating Intents

You'll recall that LUIS intents are represent actions the user wants to perform. The intent is a purpose or goal expressed in a user's input, such as booking a flight, paying a bill, or finding a news article. In our case, we'll be creating intents like sitting down, scratching, jumping, etc.

<h4 class="exercise-start">
    <b>Exercise</b>: Creating LUIS intents
</h4>

Log in to the LUIS portal at [https://luis.ai](https://luis.ai), and navigate to the *Intents* area by first navigating to the *My Apps* areas, drilling down into the *Pokemon* app:

<img src="images/chapter7/luis3.png" class="img-override" />

This page lists the various intents you have created. You'll notice that a *None* intent was automatically created for you. All LUIS apps start with this intent - you *should not* delete it. The *None* intent is used as a default fall-back intent for your LUIS apps. 

#### Finding the intents

You'll be creating a variety of intents in the *Pokemon* app. To help you, we've already defined the intents for you. In the code you downloaded from Github, locate the *language-understanding-data* folder. It contains a file named *luis-utterances.md*:

<img src="images/chapter7/luis4.png" class="img-override" />

Inside the markdown file, you'll find an intent followed by a series of utterances. For example:

```
# Sit
- ash's best friend should sit down
- sit pikachu
- sit on the floor pikachu
- have a seat meowth
- meowth please sit on the ground
```

In the snippet above, the heading `Sit` is the name of an intent you'll create, followed by utterances that align to the intent.

LUIS is like the Custom Speech Service, as it needs to *learn* the types of phrases (or utterances) that map to an intent. 

Referencing the *luis-utterances.md* file, create intents for each intent listed in the document.

Follow along below to create the first intent, then rinse and repeat for the remaining intents.

#### Adding an intent

To add an intent, click the *Create new intent* button:

<img src="images/chapter7/luis5.png" class="img-override" />

Name the intent *Sit*, as referenced in the *luis-utterances.md* file:

<img src="images/chapter7/luis6.png" class="img-override" />

On the next screen, the *Sit* intent will be listed at the top. In the text box below the intent, enter in the related utterances from the *luis-utterances.md* file. After each utterance, press *Enter* to save the utterance.

<img src="images/chapter7/intent.gif" class="img-override" />

You'll notice that the LUIS portal associated the utterance with the intent each time you press *Enter*.

When you've finished entering the associated utterances, you can scroll down to review and modify them:

<img src="images/chapter7/luis7.png" class="img-override" />

You'll also notice each utterance has a drop down next to it allow you to re-associate it with a different intent, if you made a mistake.

When you're finished entering the utterances for this intent, navigate back to the list of intents by clicking the *Intents* link on the left:

<img src="images/chapter7/luis8.png" class="img-override" />

#### Finish adding the remaining intents

Proceed to add the remaining intents listed in the *luis-utterances.md* file. When you're finished, your list of intents should look like these:

<img src="images/chapter7/luis9.png" class="img-override" />

This concludes the exercise. 

<div class="exercise-end"></div>

### Adding Entities

### Mapping Intent Phrases

### Improving Accuracy with Phrase Lists