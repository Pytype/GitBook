# 슬라이딩 윈도우 알고리즘

### 시퀀스 모델

* RNN, LSTM과 같이 시계열을 분석하는 모델을 시퀀스 모델이라고 함.

{% embed url="https://pytype.gitbook.io/wing-pytype/04.-rnn/rnn" %}

* 시퀀스 모델은 데이터의 입력을 하나의 데이터가 아닌, 여러개의 데이터가 시간 순으로 있는 배열으로 받아야 함.&#x20;
* 배열을 구성하기 위해 슬라이딩 윈도우 알고리즘을 사용.&#x20;



### 슬라이딩 윈도우 알고리즘&#x20;

* seq\_length를 7로 설정.
* 7일 동안의 데이터를 이용하여 그 다음날의 가격을 예측.

```python
def sliding_windows(data, seq_length):
    x, y = [], []

    for i in range(len(data) - seq_length):
        x.append(data[i:(i + seq_length)])
        y.append(data[i + seq_length])

    return np.array(x), np.array(y)


seq_length = 7
x, y = sliding_windows(training_data, seq_length)
```
