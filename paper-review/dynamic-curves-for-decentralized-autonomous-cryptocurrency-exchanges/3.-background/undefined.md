# 기본 함수

{% hint style="info" %}
&#x20;두 토큰 X, Y가 있는 유동성 풀.&#x20;

* x : X의 총량.&#x20;
* y : Y의 총량.&#x20;
{% endhint %}

### Mathematical relationship&#x20;

$$
y = f(x)
$$

| AMM  | Function             |
| ---- | -------------------- |
| CPMM | $$y = \frac{k}{x}$$​ |
| CSMM | $$y=c-x$$            |



### Price of the X token&#x20;

$$
p_{X}(x,y) = -\frac{dy}{dx}
$$

| AMM  | Function                     |
| ---- | ---------------------------- |
| CPMM | $$p_{X}(x,y)=\frac{k}{x^2}$$ |
| CSMM | $$p_{X}(x,y)=1$$​            |



### Value of the pool

* 토큰 Y의 가치를 기준으로 계산.&#x20;

$$
V_{p}(x,y) = p_{X}\cdot x + y
$$

| AMM  | Value of the pool            |
| ---- | ---------------------------- |
| CPMM | $$p_{X}(x,y)=\frac{k}{x^2}$$ |
| CSMM | $$p_{X}(x,y)=1$$​            |

