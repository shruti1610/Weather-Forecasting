# Weather-Forecasting

RNN and LSTM
- Import libraries and read the CSV file.
- Plot original data
- Perform split_sequence(data, n_steps) that will split the sequence of data into time window that is 20 and is also gathers input and output parts of the pattern.
- Split the data into training (1996 – 2009) , validation (2010 – 2011) and testing data(2012 – 2016)
- Train the data and make predictions using RNN and LTSM model.
- Check the performance of both the models by making data stationary.
- Calculate the RMSE value
- Evaluate the results.

RNN
>Recurrent Neural Networks or RNNs are a special type of neural network designed for sequence problems.
>The recurrent connections add state or memory to the network and allows it to learn broader abstractions from the input sequences.
>RNN is widely used for: Text data, Speech data, Classification prediction problems,  Regression prediction problems, Generative models.
>All RNNs have feedback loops,. But it can be difficult to train standard RNNs to solve problems that require learning long-term temporal dependencies. (called the vanishing gradient problem). 
>Here in SimpleRNN has just Input (xt) and Previous Output (ht-1). Passed through Tanh activation function.(No Gates are present).

LSTM
>LSTM networks are a type of RNN that uses special units in addition to standard units that include a 'memory cell' that can maintain information in memory for long periods of time. A set of gates (Forget and Output) is used to control when information enters the memory.
>The Sequential()  model is a linear stack of layers in which we can add more layers.

Comparision:
>As evaluated performance of models on original data is better then on stationary dataset.
>In  sophisticated dataset that is  stationarity, In which  cycle or trend is obvious.
>For the model to focus on the underlying signal it should be removed because, the models  itself has an  ability to learn oscillation behavior (trends).
>So this models is not as useful as, such patterns are often explicitly removed on stationary data. 
>This models have  possibility to perform well on non-stationary series.

CNN
>The nearby data points for streamline flow of Ganges will be very similar in range. Data farther away from each other has chances to change abruptly. Thus, this data is not fully connected and convolutional layer will be adequate.
>Fully connected networks result in overfitting data for CNN.
>CNN works well on large data.
>This model makes one-step predictions and outputs are fed as inputs for subsequent predictions. 

