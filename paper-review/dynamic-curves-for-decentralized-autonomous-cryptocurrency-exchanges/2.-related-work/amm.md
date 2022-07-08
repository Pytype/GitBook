# AMM의 문제점

### Slippage

#### 정의&#x20;

* 일반적인 정의 : 매매 주문 시 체결 오차로 인해 원하는 가격과 다른 가격으로 거래가 체결된 경우의 가격 차이.&#x20;
* AMM에서의 정의 : 거래 전 pool의 가격과 거래에 대해 얻은 실질적인 가격 사이의 차이.&#x20;

#### 발생 원인&#x20;

* 거래 중 토큰 가격이 변동하여 발생.
* Pool의 크기에 비해 큰거래가 발생하는 경우, 슬리피지가 급격히 증가하여 거래 이익이 감소함.&#x20;



### Impermanent Loss

* 유동성 풀에 유동성을 공급한 이후, 예치한 자산의 가격이 변화할 때 발생.&#x20;
* 유동성을 공급하지 않고, 암호화폐를 그대로 가지고 있었을 때와 비교하 손실이 발생함.
* 자산의 가격 변화가 클 수록 더 큰 비영구적 손실(IL)이 발생.&#x20;
