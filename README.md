# 🧐 데이콘 이커머스 고객 세분화 분석 아이디어 경진대회

**✅ 한 줄 소개**<br/>이커머스 데이터를 활용한 고객 맞춤형 마케팅
<br/>
<br/>
**✅ 진행 기간**<br/>2024.02
<br/>
<br/>
**✅ 팀원**<br/>3인 팀 프로젝트
<br/>
<br/>
**✅ 맡은 역할**<br/>RFM 분석 실시
<br/>
<br/>
**✅ 사용 툴**<br/>datetime, matplotlib, numpy, pandas, seaborn
<br/>
<br/>
**✅ 분석 방법**<br/>RFM, Cohort
<br/>
<br/>

## 📈 분석 요약

이커머스(전자상거래)는 직접 대면해서 거래하지 않는 시스템이기 때문에 고객이 남긴 구매 기록을 통해 어떤 고객에게 집중해야 할 지, 어떻게 서비스를 개선할 지 등을 파악해야 합니다. 

이번 프로젝트에서는 파이썬을 이용하여 다양한 소비 패턴을 지닌 고객들을 대상으로 분석할 것입니다.  고객 맞춤형 판매 전략을 제시하고, 시기나 계절성에 따라 고객의 재방문율을 높여 판매자의 이익을 얻을 수 있는 방안을 제언할 것입니다. 
<br/>
<br/>

## ✏️ 분석 내용

### **RFM 분석**

얼마나 최근에(R), 얼마나 자주(F), 얼마나 많이(M) 구매활동을 했는가에 대한 정보를 만들고, 이를 바탕으로 고객의 상태를 세분화하는 모델인 RFM을 활용해 고객을 아래와 같이 8개의 등급으로 분류했습니다.
<br/>
<aside>
💡 고객 등급

- 챔피언: 최근에 가장 많이 구매하고 지출이 많은 최우수 고객

- 잠재 충성 고객: 평균 빈도를 보이고 상당한 금액을 지출한 최근 고객

- 신규 고객: 최근성은 높지만 구매 빈도와 금액이 낮은 고객

- 잃을 수 있는 고객: 자주 구매하고 많은 금액을 지출했지만 최근에는 구매한 적이 없는 고객

- 놓치면 안 되는 고객: 자주 방문하여 구매했으나 최근에는 방문이 뜸한 고객

- 휴면 고객: 적은 금액을 소비하고 방문 빈도가 낮으며 오래 전에 방문한 고객

- 이탈 고객: 세 수치 모두 가장 낮은 고객

- 기타: 위 7개에 해당되지 않는 경우
<br/>
</aside>

### **코호트 분석**

코호트 분석은 동일한 기간 동안 동일한 특성을 가진 사람들을 모아 그룹의 고객을 추적하는 기술입니다. 고객의 재구매율을 계산함으로써 재구매율이 높은 월과 낮은 월을 살펴보고 그에 알맞은 마케팅 전략을 세우기 위해 해당 분석을 실시했습니다.
<br/>
<br/>

## 📝 분석 결과

### RFM 분석

![RFM](https://github.com/user-attachments/assets/1533d865-b35a-42dc-9f38-97ce7834ee42)

RFM 분석 결과, 잠재 충성 고객의 비중이 가장 높았고 그 뒤로 잃을 수 있는 고객, 기타, 이탈 고객, 신규 고객, 휴면 고객, 챔피언 고객, 놓치면 안 되는 고객의 순으로 비중이 나타났습니다.
<br/>

### 코호트 분석

![Cohort](https://github.com/user-attachments/assets/73ef3ec2-5de9-4f98-9708-28aeee4bc13a)

초기 재구매율보다 마지막 재구매율이 높은 2019년 1월과 2월에 중점을 두었습니다.

- 2019년 1월 : 첫 구매 이후 4, 6개월이 지난 시점을 제외하곤 꾸준히 증가했으며, 7개월이 지난 시점에 재구매율이 21.9%로 가장 높은 증가율을 보였으나 8개월 이후부터는 다시 감소했습니다.
- 2019년 2월 : 첫 구매 이후 5개월까지 재구매율이 꾸준히 상승하다 감소했습니다. 그 후 계속 감소하다가 10개월이 지난 이후 16.7%로 다시 증가했습니다.

전체적으로 늦겨울에서 봄 정도는 2-3월에 재방문율이 높으며, 여름에서 가을 정도인 8-9월에 재방문율이 낮았습니다.
<br/>
<br/>

## 📝 결과 활용

- **고객 세그먼트별 솔루션 제공** : 위에서 설정한 고객 세분화 기준과 RFM 분석 결과를 바탕으로 할인 행사를 진행하는 등 고객을 유지하기 위한 마케팅 전략을 세울 수 있습니다.
- **재구매율 그룹 타겟 마케팅** : 재구매율이 높은 그룹에 대해서는 마케팅 전략을 강화하고 재구매율이 낮은 그룹에 대해서는 이탈 원인을 조사하여 문제점을 파악해볼 수 있습니다. 또한 계절의 특성을 반영하여 판매 전략을 세울 수 있습니다.
<br/>
<br/>

## 😀 성장 경험

- 고객의 분포와 특성에 따라 다양하게 세분화할 수 있다는 점을 배웠고, 고객 맞춤형 마케팅 전략을 직접 세울 수 있다는 점에서 유익한 프로젝트 경험이었습니다.
- 마케팅 데이터 분석에 자주 쓰이는 분석 기법을 이번 프로젝트를 통해 익힐 수 있었습니다.
<br/>
<br/>

## 😅 아쉬운 점

구매 물품 카테고리에 대한 설명이 명확하지 않았고 실존하지 않는 카테고리도 존재하여 깊이 있는 인사이트를 도출하는 것에 어려움을 겪었습니다.
