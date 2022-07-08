# Train/Test 데이터

### Train data

* 총 1331개의 데이터 중 800개를 Train에 사용.&#x20;

```python
from torch.autograd import Variable

dataX = Variable(torch.Tensor(np.array(x)))
dataY = Variable(torch.Tensor(np.array(y)))

train_size = 800
trainX = Variable(torch.Tensor(np.array(x[0:train_size])))
trainY = Variable(torch.Tensor(np.array(y[0:train_size])))
```



### Test data

* 나머지 데이터를 모델을 평가하기 위해 사용.&#x20;

```python
test_size = len(y) - train_size
testX = Variable(torch.Tensor(np.array(x[train_size:len(x)])))
testY = Variable(torch.Tensor(np.array(y[train_size:len(y)])))
```

