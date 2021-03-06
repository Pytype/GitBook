# 목적

### AMM의 한계

* external arbitrageurs, 차익 거래자의 필요 -> DEX의 LP에 있는 토큰의 가격을 시장 가격과 맞춤.&#x20;
* 시장 가격이 급격히 변하게 되면, 유동성이 낮아지고 LP의 총 가치가 감소될 수 있음.&#x20;



### 문제점 해결&#x20;

* AMM을 정적(static) 방식이 아닌 동적(dynamic curves)로 구성.&#x20;
* 시장가격 오라클 입력을 바탕으로, 자산 간의 수학적 관계를 수정하여 LP의 가격이 시장가격과 동일하도록 조정.&#x20;

{% hint style="info" %}
오라클(Oracle) :  블록체인 밖에 있는 데이터를 블록체인 안으로 가져오는 것
{% endhint %}

* 차익 거래 기회를 제거, 모든 자산에 대한 LP의 유동성 및 LP의 총 가치 유지.&#x20;
