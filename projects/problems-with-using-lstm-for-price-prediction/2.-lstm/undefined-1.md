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





