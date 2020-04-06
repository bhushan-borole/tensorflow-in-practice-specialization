# Week 1 Quiz

1. What is the name of the object used to tokenize sentences?
    - [ ] CharacterTokenizer
    - [x] Tokenizer
    - [ ] TextTokenizer
    - [ ] WordTokenizer

2. What is the name of the method used to tokenize a list of sentences?
    - [ ] tokenize(sentences)
    - [ ] fit_to_text(sentences)
    - [x] fit_on_texts(sentences)
    - [ ] tokenize_on_text(sentences)

3. Once you have the corpus tokenized, what’s the method used to encode a list of sentences to use those tokens?
    - [ ] text_to_sequences(sentences)
    - [ ] text_to_tokens(sentences)
    - [ ] texts_to_tokens(sentences)
    - [x] texts_to_sequences(sentences)

4. When initializing the tokenizer, how to you specify a token to use for unknown words?
    - [ ] unknown_token=< Token>
    - [x] oov_token=< Token>
    - [ ] unknown_word=< Token>
    - [ ] out_of_vocab=< Token>

5. If you don’t use a token for out of vocabulary words, what happens at encoding?
    - [x] The word isn’t encoded, and is skipped in the sequence
    - [ ] The word isn’t encoded, and is replaced by a zero in the sequence
    - [ ] The word isn’t encoded, and the sequencing ends
    - [ ] The word is replaced by the most common token

6. If you have a number of sequences of different lengths, how do you ensure that they are understood when fed into a neural network?
    - [x] Use the pad_sequences object from the tensorflow.keras.preprocessing.sequence namespace
    - [ ] Process them on the input layer of the Neural Network using the pad_sequences property
    - [ ] Specify the input layer of the Neural Network to expect different sizes with dynamic_length
    - [ ] Make sure that they are all the same length using the pad_sequences method of the tokenizer

7. If you have a number of sequences of different length, and call pad_sequences on them, what’s the default result?
    - [ ] They’ll get cropped to the length of the shortest sequence
    - [ ] Nothing, they’ll remain unchanged
    - [x] They’ll get padded to the length of the longest sequence by adding zeros to the beginning of shorter ones
    - [ ] They’ll get padded to the length of the longest sequence by adding zeros to the end of shorter ones

8. When padding sequences, if you want the padding to be at the end of the sequence, how do you do it?
    - [ ] Pass padding=’after’ to pad_sequences when initializing it
    - [x] Pass padding=’post’ to pad_sequences when initializing it
    - [ ] Call the padding method of the pad_sequences object, passing it ‘after’
    - [ ] Call the padding method of the pad_sequences object, passing it ‘post’