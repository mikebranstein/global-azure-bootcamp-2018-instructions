## Building Custom Speech Service data sets 

In this chapter, you'll learn:
- The difference between training and testing data sets
- How acoustic data sets are built 
- That language data sets help the Custom Speech Service (CSS) understand the likelihood of certain words and phrases
- That pronunciation data sets can help with simple word and and syllable replacements

### Understanding Machine Learning Data Sets

At the core of every artificial intelligence (or machine learning) problem is data. And that data is used in various capacities to train, build, and test the systems you develop. Because data is so critical to machine learning endeavors, you'll need to learn about the different ways data is used.

> **Thank you, StackExchange**
>
> This next section was adapted from a [StackExchange post](https://stats.stackexchange.com/questions/19048/what-is-the-difference-between-test-set-and-validation-set). Thank you to all that contributed, as you said it better than I could have.

#### Training and Test Data Sets

In many machine learning processes, you need two types of data sets:

- In one data set (your *gold standard*) you have the input data together with correct/expected output, This data set is usually duly prepared either by humans or by collecting some data in semi-automated way. But it is important that you have the expected output for every data row here, because you need to feed the machine learning algorithms the *expected*, or *correct* results for it to learn. This data set is often referred to as the *training data set*. 

- In the other data set, you collect the data you are going to apply your model to. In many cases this is the data where you are interested for the output of your model and thus you don't have any "expected" output here yet. This is often real-world data. 

With these two data sets, the machine learning process adheres to a standard 3-phase process:

1. Training phase: you present your data from your "gold standard" (or *training* data set) and train your model, by pairing the input with expected output. Often you split your entire training data set into two pieces. Approximately 70% of the training data is used for training, and 30% reserved for validation/testing. The 30% reserved data is often referred to as *test* data. The result of this phase is a trained model.

2. Validation/Test phase: to estimate how well your trained model has been trained, you pass in the reserved 30% of your testing data and evaluate it's accuracy. 

3. Application phase: now you apply your trained model to the real-world data and get the results. Since you normally don't have any reference value in this type of data, you can only speculate about the quality of your model output using the results of your validation phase. You perform additional accuracy tests.

> **Separation of Training, Test, and Real-World Data Sets**
>
> An easy mistake to make with your training, test, and real-world data sets is overlapping data (or reusing data from one set in another). Imagine that you training a model to answer true/false questions using a series of 10 questions and answers. After the model is trained, you use the same 10 questions to evaluate how well the model performs. Ideally, it should perform 100%, but you don't know how well it *really* performs because you tested with the training data. The only true test is to use other real-world questions, then re-evaluate its performance.

#### Applying Machine Learning Data Set Concepts to the Custom Speech Service

Now that you know about the different types of data, you'll be creating training data sets for acoustic, language, and pronunciation data, then testing acoustic data. 

> **Acoustic, Language, and Pronunciation**
>
> Don't worry if you don't know the difference between these 3 types of data the CSS uses, you'll be learning about it next.

### Acoustic Training data sets

### Language Training data sets

### Pronunciation Training data sets

### Acoustic Testing data sets