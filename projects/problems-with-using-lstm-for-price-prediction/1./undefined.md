# 데이터 구성

### 데이터 가져오기&#x20;

{% embed url="https://finance.yahoo.com/quote/BTC-USD/" %}

{% embed url="https://finance.yahoo.com/quote/ETH-USD/" %}

* 2018-03-27 \~ 2021-11-16 기간 동안의 비트코인(BTC), 이더리움(ETH) 가격 데이터를 각각 csv 파일로 저장.&#x20;

{% tabs %}
{% tab title="BTC 가격" %}

{% endtab %}

{% tab title="ETH 가격" %}

{% endtab %}
{% endtabs %}



### 데이터 정규화&#x20;

* 레이블을 제외하면 $$1331 \times 2$$ 크기의 데이터.&#x20;
* 1열은 20XX-XX-XX 형식의 날짜 데이터, 2열은 float 형의 가격 데이터.&#x20;



* Pandas 라이브러리와 MinMaxScaler를 이용하여 csv 파일의 가격 데이터를 추출하여 정규화.

```python
import pandas as pd
from sklearn.preprocessing import MinMaxScaler

training_set = pd.read_csv('./BTC_Price.csv').iloc[:, 1:2].values

sc = MinMaxScaler()
training_data = sc.fit_transform(training_set)
```

