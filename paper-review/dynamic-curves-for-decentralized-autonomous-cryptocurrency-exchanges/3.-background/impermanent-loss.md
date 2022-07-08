# Impermanent Loss 함수

* 거래가 이루어지면서, 가격의 변화가 일어남.&#x20;
* Value of the pool (V)의 값이 감소하게 됨.&#x20;
* V값 감소를 상대적 비율로 나타낸 값을  divergence loss 또는 Impermanent Loss (δ)로 표현.&#x20;

$$
\delta = \frac{V_{p_n}(x_n, y_n)-V_{p_n}(x_0, y_0)}{V_{p_n}(x_0, y_0)}
$$



### CPMM의 Impermanent Loss&#x20;

$$
V_{p_n}(x_n, y_n)=2\sqrt{k\cdot p_n},\, \, \, \, \, \, V_{p_n}(x_0, y_0) = p_n\sqrt{\frac{k}{p_0}} + \sqrt{k\cdot p_0}
$$

$$
\delta = \frac{2\sqrt{\rho}-1-\rho}{1+\rho}\, \, \, \, \, \, \, \, \, \, \left ( \rho  = \frac{p_n}{p_0} \right )
$$

​

### CSMM의 Impermanent Loss&#x20;

$$
V_{p_n}(x_n, y_n)=V_{p_n}(x_0, y_0)=c
$$

$$
\delta = 0
$$





