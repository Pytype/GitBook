# LMSR

* Hanson’s logarithmic market scoring rules.&#x20;
* 예측 시장에서 낮은 유동성 및 거래량 문제를 해결하기 위해서 사용.&#x20;
* 이러한 LMSR을 기반으로 한 LMSR-based AMM도 DeFi 시장에 등장함.&#x20;



### (extra) Functions in  LMSR

* The cost function

$$
C\left ( \mathbf{q}\left ( x_{n}, y_{n} \right ) \right )=b\cdot \textrm{ln} \left ( e^{x_{n}/b}+e^{y_{n}/b} \right )=k
$$

$$
y_{n}=b\cdot \textrm{ln}\left ( e^{k/b} - e^{x_{n}/b} \right )
$$

* The asset value of the pair

$$
V\left ( \mathbf{q}_{n}\left ( x_{n}, y_{n} \right ) \right )=2\cdot b\cdot \textrm{ln} \left ( e^{k/b}-e^{x_{n}/b} \right )
$$



#### reference

1\)

{% embed url="https://augur.mystrikingly.com/blog/augur-s-automated-market-maker-the-ls-lmsr" %}

2\)

Impermanent Loss and Gain of Automated Market Maker Smart Contracts (Hyoung Joong Kim, Member, IEEE, Soohyuk Choi, Yong Tae Yoon, Shiyong Yoo, Member, IEEE)

​
