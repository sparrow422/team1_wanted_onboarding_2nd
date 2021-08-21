# 모두의 주차장 DB 분석

## ⚽ Goal
  * COUNT에 대한 EDA
  * 요일 별 EDA
  * COUNT 예측 모델링

## 📊 EDA
 * **전체 컬럼의 의미 파악**
   - 전체 컬럼은 USER_ID, JOIN_DATE, D_TYPE, STORE_ID, GOODS_TYPE, DATE, COUNT, AD1
   - 여기서 쉽게 추론이 가능한 항목은 USER_ID, JOIN_DATE, STORE_ID, DATE이며 각각 사용자 ID, 가입날짜, 주차장 ID, 결제 날짜이다.
   - D_TYPE은 의미는 정확히 알 수 없으나 AA, BB와 달리 CC는 높은 COUNT값을 가지고 있다. 따라서 기간권 사용자이거나 VIP 유저등을 나타낸다고 생각된다.
   - GOODS_TYPE은 이름에서 결제 수단이나 구매상품과 관련되어있다고 생각되는데 COUNT값과는 유의미한 상관관계가 없다.
   - COUNT는 처음엔 이용횟수라고 생각되었으나 이용횟수일 경우 사용자나 주차장, 날짜 등에 대하여 누적되는 양상을 보여야하지만 전혀 그렇지 않았고 이용시간이라고 추측된다.
   - AD1은 주차장 ID와 관련된 모습을 보여 주소에 관한 코드로 보인다.

* 
