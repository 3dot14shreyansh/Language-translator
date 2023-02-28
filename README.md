# Attention Model
![My Image](images/my-image.jpg) 

### Need of Attention models: 
- LSTM is not accurate when it comes to generate long range vector context (long sentences).
- The ***vector W*** will have more context which are near to ***vector W*** like and ***vector D*** or ***vector C***.

### Attention Models:
- Instead of using Uni-directional LSTM RNN, attention model uses Bi-directional LSTM RNN.
- However Encoder uses Bi-directional LSTM RNN but Decoder does not use the same.
- In this case the model will get the information context of future words or will contain the vector imformation of previous words in case on long sentences.
- Attention model is capable of preserving the context because of a hyper-parameter WINDOW.
- The number of activation constant 'α' is equal to number of windows allowed.
- The scope of 'α' will determine the lenght of sentence gets translate at a time. 
- The sum of 'α' under a window size will always be equal to 1. It is the ***Softmax Function*** which helps any number of 'α' with sum as 1.
- Context vector on decoder side is genrated using output of Bi-directional LSTM RNN and 'α' values. This is similar to ***Feed Forward Neural Network.***


### Acknowledgement: 
- Research paper : Neural machine translation by jointly learning to align and translate (ICLR 2015) by Dzmitry Bahdanau, KyungHyun Cho and Yoshua Bengio. [Link to asset.](https://arxiv.org/pdf/1409.0473.pdf)
- Research paper :Multilingual distributed representations without word alignment. In Proceedings of the Second International Conference on Learning Representations (ICLR 2014) by Hermann K and Blunsom P.

