# AMM의 등장 배경

### 기존 암호화폐 거래소

* 중앙화(centralized) 되어 있음.
* order book mechanism 사용.

{% hint style="info" %}
오더북 : 매도자와 매수자들이 원하는 가격과 수량을 보여주는 도표, 원하는 가격과 수량이 일치하면 그 지점에서 주식 매매가 이루어진다.
{% endhint %}

{% hint style="danger" %}
문제점

1. financial power이 분산되지 않고 집중되어 있다.&#x20;
2. 단일 장애점(SPOF)의 발생이 쉬워 공격을 당할 시 많은 자금의 손실이 발생한다.
3. 시가 총액이 작은 토큰의 경우, 유동성 문제로 인해 금융 시장 진입 장벽이 있다.
{% endhint %}



### DEX에서 오더북 구현의 어려움

* 스마트 계약의 형태로 탈중앙화된 방식으로 오더북을 구현함.&#x20;
* 높은 gas 비용의 문제 & 매칭 알고리즘 구현의 어려움.&#x20;



##
