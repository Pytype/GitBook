# Simulation

### Simulation

{% hint style="info" %}
1000개의 X 토큰, 1000개의 Y 토큰을 각각 보유하고 있는 LP, trader, 차익거래자.&#x20;

거래는 정규분포를 바탕으로 랜덤하게 발생. (랜덤 은 4가지 AMM에 동일하게 적용).&#x20;

시장 가격은 0에서 10까지 선형적으로 증가.&#x20;
{% endhint %}

#### 결과

![](../../../.gitbook/assets/Simulation\_01.PNG)

![](../../../.gitbook/assets/Simulation\_02.PNG)

![](../../../.gitbook/assets/Simulation\_03.PNG)

![](../../../.gitbook/assets/Simulation\_04.PNG)

####

#### 결과 해석

* CSMM에서 초기 조건의 pool price가 market price보다 높아서 차익거래가 발생, market price가 pool price를 넘는 순간 simulation이 중단
* 2개의 static AMM에서는 pool price와 market price의 차이가 있어서 차익거래가 발생하지만, dynamic AMM에서는 지속적으로 pool price가 market price와 같게끔 조정되어 차익거래가 발생하지 않음.&#x20;
* Dynamic CSMM, CPMM의 그래프에서, Theorem 1처럼 Slippage loss에 해당하는 가치만큼 LP의 가치가 올라감을 확인함. (그래프가 대칭적)
* Dynamic CSMM, CPMM의 LP 가치 변동은 static AMM과 비교하여 매우 적은 수준을 유지함 (원래 가치의 85% 이상을 보존함.)&#x20;
* Dynamic CPMM은 Dynamic CSMM과 비교해서  slippage가 크기 때문에 규모가 큰 거래가 잘 일어나지 않아야함 (하지만, 이 simluation에서는 동일한 random을 설정하여 확인 불가능)



