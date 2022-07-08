# 모델 학습

### Epoch, Learning rate 설정&#x20;

```python
num_epochs = 1500
learning_rate = 0.01
```



### Cost 함수, Optimizer 설정

```python
criterion = torch.nn.MSELoss()
optimizer = torch.optim.Adam(lstm.parameters(), lr=learning_rate)
```



### 학습&#x20;

```python
for epoch in range(num_epochs+1):
    outputs = lstm(trainX)
    optimizer.zero_grad()

    loss = criterion(outputs, trainY)
    loss.backward()

    optimizer.step()

    if epoch % 100 == 0:
        print("Epoch: %d, loss: %1.5f" % (epoch, loss.item()))
```



### 결과 그래프&#x20;

```python
import matplotlib.pyplot as plt

lstm.eval()
train_predict = lstm(dataX)

data_predict = train_predict.data.numpy()
dataY_plot = dataY.data.numpy()

data_predict = sc.inverse_transform(data_predict)
dataY_plot = sc.inverse_transform(dataY_plot)

time_label_num = [n for n in range(1331) if n % 100 == 0]
time_label_text = ['Mar 27, 2018', 'Jul 05, 2018', 'Oct 13, 2018', 'Jan 21, 2019',
                   'May 01, 2019', 'Aug 09, 2019', 'Nov 17, 2019', 'Fev 25, 2020',
                   'Jun 04, 2020', 'Sep 12, 2020', 'Dec 21, 2020', 'Mar 31, 2021',
                   'Jul 09, 2021', 'Oct 17, 2021']

plt.title('BTC Price Prediction (with real price data)', fontweight="bold")
plt.xlabel('Time')
plt.xticks(time_label_num, labels=time_label_text, rotation=28)
plt.ylabel('Price ($)')
plt.plot(dataY_plot, label='Real Price')
plt.plot(data_predict, label='Predicted Price')
plt.axvline(x=train_size, c='r', linestyle='--')
plt.legend()
plt.tight_layout()
plt.show()
```

