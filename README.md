# Stock Market Prediction - LSTM
Predicting stock prices is a challenging task due to the complexity and volatility of the stock market. Various methods can be used for this purpose, ranging from statistical techniques to machine learning models. One popular and effective method is using `Long Short-Term Memory (LSTM) networks`, a type of `recurrent neural network (RNN)` specifically designed to capture temporal dependencies in sequential data.

# LSTM
LSTM networks are a type of RNN designed to overcome the limitations of traditional RNNs, which struggle with learning long-term dependencies due to the [vanishing gradient problem](https://youtu.be/qhXZsFVxGKo?si=J4p0qo0h1X9Nk7EM). LSTMs address this by using a memory cell that can maintain information over long periods. This makes LSTMs particularly well-suited for time series prediction tasks, such as stock price forecasting.

<div align="center">
<img src="https://github.com/ShayanDarabi/Stock-Market-Prediction-LSTM/blob/main/LSTM.webp" alt="Stock Prices" width="600">
</div>

### Key Features of LSTM

1. **Memory Cells**:
   - LSTM networks have memory cells that can maintain information over long periods. These cells help the network remember values over arbitrary time intervals, effectively addressing the vanishing gradient problem present in traditional RNNs.

2. **Gates**:
   - LSTMs use special units called gates to control the flow of information. There are three main gates:
     - **Input Gate**: Controls how much of the new information from the current input is used to update the cell state.
     - **Forget Gate**: Decides what portion of the previous cell state should be forgotten.
     - **Output Gate**: Determines the output based on the cell state and the current input.

3. **Cell State**:
   - The cell state is the internal memory of the LSTM, which is modified by the gates. It allows the network to carry relevant information throughout the processing of sequences, making it possible to learn long-term dependencies.

4. **Non-Linearity**:
   - LSTM units typically use activation functions like the sigmoid and hyperbolic tangent (tanh) functions. These non-linearities enable the model to capture complex patterns in the data.

5. **Ability to Capture Long-Term Dependencies**:
   - Due to its architecture, LSTM can effectively learn and remember over long sequences, capturing long-term dependencies better than traditional RNNs.

6. **Gradient Flow**:
   - By having a more controlled flow of gradients through the network via the gates, LSTM helps in reducing the issues of vanishing and exploding gradients, which are common in standard RNNs.

7. **Sequence Processing**:
   - LSTMs are designed to process sequential data, making them suitable for time series forecasting, natural language processing, speech recognition, and other tasks that involve sequential dependencies.

For more details about LSTM architecture, I recommend this page: *[Understanding LSTM Networks](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)*

# LSTM Application in Stock Price Prediction

