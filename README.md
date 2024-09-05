# Minor_Project
Word's Spell Check using NLP
This project is composed of two parts;
1 . A trained RNN (LSTM) and
2 . A character level bigram model. 
LSTM is used to query with a misspelledword in order to find a correct word.
With bigram, new query words are generated from the misspelled word, so that trained network can be queried with these generated words.
Using these new query words we expect to increase the correction accuracy.
For LSTM training,words are encoded similar to RNN.
A given word’s first letter, end letter and in between letters are encoded to 3 input vectors and compose a sequence.
Different than RNN, previous two words are not used as time steps.
Instead, a sequence of 3 vectors that are computed from a word is used. 
So any word correction is only based on its character sequence.
A given misspelled word is used to query the trained LSTM network in order to find the desired word.
Long Short-term Memory (LSTM) has shown to give an extraordinary result in solving sequential problems, including spelling correction.

Programming Language: python 
Platform: Spyder

# Spell check using NLP
### Prerequisites

First thing which you need to install is textblob library
<!--Install library-->
>pip install textblob

>import sys 
<!--command-->
>!{sys.executable} -m pip install textblob 

### How to run the script

You can first install the textblob library and then you can run the python script.
