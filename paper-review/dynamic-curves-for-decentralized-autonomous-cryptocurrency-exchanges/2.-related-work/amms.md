# AMMs

### Bancor

* AMM을 활용한 최초의 DEX.&#x20;
* 단 하나의 토큰 (BNT)를 활용한 여러 개의 유동성 풀.&#x20;
* 일반적인 AMM (two-asset curve based AMM)과는 다르게, 두 암호화폐가 직접적으로 교환되지는 않음.



### Constant Product Market Maker

* 유니스왑에서 사용되는 함수.
* 수량의 곱이 일정하다고 함수를 정의.&#x20;
* 슬리피지(Slippage) 문제 : 교환하고자 하는 토큰 수량이 많을수록 더 큰 손해를 보게 됨.&#x20;
* 이론적으로 무한대의 유동성을 제공.&#x20;

$$
x\cdot y=k
$$

![https://medium.com/bollinger-investment-group/constant-function-market-makers-defis-zero-to-one-innovation-968f77022159](https://miro.medium.com/max/1334/1\*RRKqLQWEeUJXcjuvs5vHlQ.png)



### Constant Sum Market Maker

* 수량의 합이 일정하다고 함수를 정의.&#x20;
* 무한한 유동성을 제공하지는 못하는 문제점.&#x20;

$$
x+y=k
$$

![https://medium.com/bollinger-investment-group/constant-function-market-makers-defis-zero-to-one-innovation-968f77022159](https://miro.medium.com/max/1400/1\*OXxOE-Cu78TSeMwMKhy33Q.png)



### StableSwap/Curve

* Constant Sum, Constant Product의 두 방식이 혼합된 형태.&#x20;
* CPMM의 슬리피지 문제와, CSMM의 유동성 문제를 어느 정도 해결하면서 두 모델의 장점을 이용.&#x20;

{% hint style="info" %}
* LP의 규모가 작은 경우, Constant Product와 유사하게 동작.
* LP의 규모가 큰 경우, Constant Sum와 유사하게 동작.
{% endhint %}

![https://medium.com/berryfi/curve-finance%EC%9D%98-stableswap-8f66cdb68be7](https://miro.medium.com/max/1166/1\*iALGAXbkoQ2qmz-s1d5oKg.png)



### Constant Ellipse Market Maker

$$
(x-a)^2 + (y-a)^2+b\cdot xy=C
$$



### (extra) Constant Mean Market Maker

* Constant Product에 weight을 적용한 Curve
* 가중치가 적용된 두 개 이상의 asset을 허용함.&#x20;

![https://medium.com/bollinger-investment-group/constant-function-market-makers-defis-zero-to-one-innovation-968f77022159](https://miro.medium.com/max/1400/1\*7sRWd3Pmjf7Zp2NGAK-YSQ.png)

