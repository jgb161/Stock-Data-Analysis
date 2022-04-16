# Stock-Data-Analysis
Created By: Matt Rivas, Jeremy Brown, Dana Smith 

Mission
To predict future closing process for TSLA and AAPL stock, through GRU, Q Learning and LSTM models.

Model Clean Up, Data training Summary
1. We imported 12 years  of TSLA  stock data & 22 years of AAPL stock data. 

2. After looking at some of the graphs, we determined it was more efficient to analyze the last 4 years of TSLA & last 6 years of AAPL
Q Learning model was more based on a plug and play of GAMMA and Epsilon variables. The lower the GAMMA and the higher the GAMMA the worse the total rewards were
We found a sweet spot in the 70% range.

3. In our LSTM model:
We adjusted the training & testing percent between 70 - 90%
Adjusted epochs & batches 

GRU model: 
Examples of training and clean up processes
Attempted to predict pricing of stocks using historical data

GRU TSLA ANALYSIS
Used 1024 points of historical stock data
Below is the accuracy graph of the training model.
As we can see, GRU did a poor job anticipating price movement. 
This poor performance can be explained by lack causality ie yesterdays stock price does not influence the stock price in the future

AAPL GRU Analysis 
While the true trend of AAPL seems to be more closely correlated to some of the forecasts, the results aren’t predictive enough to be relied upon. Specifically forecast 5 seems to have been the most correlated. Perhaps with more refinement this model could have more accurately predicted AAPL price. 

LSTM
* Similar to GRU model, LSTM was created as a solution to short-term memory or vanishing gradient problems that appear while training RNN’s with long data sequences

* Historical & current data are combined 

* Data is then ran through a layers to sort out non-relevant data and decides what data should be added 

*LSTM can choose which information is relevant to remember or forget during sequence process  

REinforcement Learning - QLearning
⦁ Seeks to learn a policy that maximizes its total reward

* A q-table is created to assign values to each state and action as a reference point for it to select its next best actio

⦁ Agent interacts with environment and updates q-table to reflect whether or not the reward was positive or negative

⦁ Common variable in Q-Learning models is gamma, or the discount factor, and it helps assess what the future rewards will be

⦁ Epsilon is another common variable, and it determines how aggressive or greedy the model will be seeking

Conclusion:

If we had more time, we would have done a social media anaylsis to determine if certain keywords affected the stock prices in a positive or negative manner

We would have created a Dashboard if we had more time

Q-Learning model predicited whether it would be a buy or sell, while GRU & LSTM were used to help predict pricing fluctuations.

Q-Learning AAPL model averaged at 9% and TSLA earning 21%, which we would be better buying and holding until the end. 

Historical stock data is not predictive of future stock prices, which is why LSTM & GRU were not good predictive models.






