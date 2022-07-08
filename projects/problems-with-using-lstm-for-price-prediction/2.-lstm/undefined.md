# 모델 평가

### 평가 및 그래프

![](../../../.gitbook/assets/result2.PNG)

```python
lstm.eval()
train_predict = lstm(dataX)

data_predict = train_predict.data.numpy()
dataY_plot = dataY.data.numpy()

data_predict = sc.inverse_transform(data_predict)
dataY_plot = sc.inverse_transform(dataY_plot)


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

