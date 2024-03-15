# Machine Translation

This project implements a Sequence-to-Sequence machine translation model using an encoder-decoder LSTM network with Luong-style attention. The implementation was done using the [Keras Functional API](https://keras.io/guides/functional_api/).

The implementation of this project is based on the tutorial provided by [Francois Chollet's Blog](https://blog.keras.io/a-ten-minute-introduction-to-sequence-to-sequence-learning-in-keras.html). The blog provides detailed explanations of Seq2Seq models, encoder-decoder architectures, and code examples, which were helpful in developing this project. Make sure to check out the blog for more information and detailed explanations.

The data used to train the model (English to French) was obtained from [here](http://www.manythings.org/anki/). It contains translations for many other languages as well, which can be used interchangeably with the current training data to train translation models for different languages.

## Project Content

- `EncDec.ipynb`: Contains the model for machine translation from English to French. The notebook includes implementations of both Seq2Seq models with and without attention. However, the inference part present in the notebook is tailored for the attention model and may need adjustments if attention is not used. Check out the blog link provided above for guidance.
- `s2s_model.keras`: Contains the saved model trained on the English to French data. It can be loaded directly, and the notebook contains code to do so.

## Requirements

- TensorFlow version 2.10.1
- Keras version 2.10.0
- NumPy

(Note: TensorFlow versions above 2.10 are not supported on GPU on Windows Native, which is why these specific versions were used.)

