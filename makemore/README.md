### Makemore
As the name suggests, makemore makes more of things what you give it!!!

For example: if we take the dataset of lots of names, and if we train makemore on this dataset, it will learn to make more of things like this: And in this particular case, it will make more things that sound name-like but are actual unique names.
May be you wish to come up with cool sounding unique name, you can use this.


Under the hood, makemore is a **Character Level Language Model** : - which means it treats every single line in the input data set as an example and within each example, it is treating them all as sequences of individual characters:
For example: if an line in the dataset is "Ganitagya", then the line will be an example and 'G', 'a', 'n', 'i', 't', 'a', 'g', 'y', 'a' will be the sequence of characters.

Hence **Character Level Language Model** is modeling those sequences of characters and knows how to predict the next character in the sequence

We would be implementing the following character level language models in terms of the neural networks that are involved in predicting the next character in a sequence 
1. Bigram (One character simply predicts the next one with a lookup table of counts)
2. Bag of Words 
3. MLP (Muli Layer Perceptrons)
4. Recurrent Neural Networks (RNN)
5. Modern Transformers (Somewhat equivalent to gpt2)


Extension of the project: 
After the character level , we will get into word level sequence and its predictions so that we can generate documents of words not just little segments of characters.
Then we will get into images; image text networks such as Dolly, stable diffusion, etc.

We first work in `build_makemore.ipynb` and then going for an alternative way of solving the problem in `build_makemore_nn.ipynb`


Reference:
1. https://www.youtube.com/watch?v=PaCmpygFfXo&list=PLAqhIrjkxbuWI23v9cThsA9GvCAUhRvKZ&index=2

References for Dataset;
1. https://www.kaggle.com/datasets/surajpratap/sixty-thousand-unique-indian-names-dataset
2. https://github.com/balasahebgulave/Dataset-indian-names/blob/master/Indian_Names.csv