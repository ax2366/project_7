# 종업원 이탈 예측 모델 (IBM HR 데이터를 바탕으로)


- 사용 데이터 : IBM HR Analytics Employee Attrition & Performance

- 목적 : 인재 이탈 예측 + 종업원 고용 비용 절감 위해 데이터 분석 진행

- 타겟 : 이탈 여부

- 퇴사자(이탈) 비율 : 약 16%

- 상관관계
  월 소득 - job level : 0.95  /  총 근속 연수 - job level : 0.78  /  성과 평가 - 급여 인상 : 0.77  등

- 빅쿼리 XGBoost 사용 -> 테스트 정확도 : 0.89

- 주피터 XGBoost 사용  ->  테스트 정확도 : 0.89

- 테스트 진행 -> 종업원 이탈 예측  (특성 및 순열 중요도가 높은 5개 피처의 값을 바꿔가며 진행) 
  결과값 0 반환 -> 이탈 예정 O   /  결과값 1 반환 -> 이탈 예정 X 

- 비즈니스 인사이트
  - 부서 – 월급에 따른 이탈 예정 분류 모델 제작  유의미한 관계가 있다는 것을 발견  월급뿐만 아니라 여러 방안이 필요 
  - 사내 문화 개편 방법 제안
  - 핵심 인재 이탈 예방 : 실적에 따른 성과급 지급 방법 제안
