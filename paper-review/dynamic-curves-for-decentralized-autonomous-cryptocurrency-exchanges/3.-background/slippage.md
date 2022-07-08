# Slippage 함수

| X 토큰 구매량 | ∆x             |
| -------- | -------------- |
| 거래 전 LP  | $$(x_0, y_0)$$ |
| 거래 후 LP  | $$(x_n, y_n)$$ |

$$
x_n=x_0-\Delta x
$$

* 거래 전 예상 지불 가격&#x20;

$$
\Delta y_0 = p_0\Delta x
$$

* 거래 후 실제 지불 가격&#x20;

$$
\Delta y = y_n-y_0
$$

* Slippage

$$
S(x_0, y_0, \Delta x) = \Delta y - \Delta y_0
$$

{% hint style="info" %}
CSMM의 경우 Slippage 값이 0
{% endhint %}

