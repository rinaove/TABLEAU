# 🎨 태블로 5주차
- 이번주 목표

## 20. 필터

<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/8cc806b6-6c0d-47cc-9b0b-c3582f2effb7" />

<img width="640" height="501" alt="image" src="https://github.com/user-attachments/assets/8d1a3317-3d95-48d9-9dd4-ce743c72656c" />

* 범례 > 숨기기 (테이블에서 누계 구성 비율이 변경되지 않음)
<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/f6db4479-344e-474c-ad8b-217f2aa4078c" />


## 21. 이중축
* 행값에 있는 변수 우클릭 > 이중축 선택
  * 각각의 마크값이 생김
  * 축 동기화를 해야 양쪽 스케일값이 맞춰짐
  * 그러나, 양쪽 값 차이가 큰 경우 축 동기화 시 한쪽 범위가 안보일 수 있음
<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/af705be9-f17f-46bb-a5fd-37c52471691a" />
<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/6f665d9f-7664-4dca-bdd1-db500f000dfb" />

* combinded axis 차트
<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/5bd27769-9c65-4424-8042-5f087ccd626e" />

* 이중축의 장점: 각 변수값 커스터마이징 가능 (마크값이 2개라서)
* combinded axis 차트: 한 컬럼 안에 2개의 변수값을 두고 이중축을 설정할 수 있다는 점

<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/145f2f27-3994-4b11-a58e-74f0ced003ad" />
<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/83bb0a85-ca4f-4820-b3df-b03c22ba1446" />


## 22. 분석 패널
* 패널: 셀과 테이블 중간
* 상수 라인: 원하는 값을 라인으로 지정 (Order date도 가능)

<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/2682ecbb-74dd-40f6-a53b-0751f47c894c" />

* 태블로 예측기법: 지수평활법
 * 불연속형도 가능  

<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/bd44700b-3ae9-4e6e-b4c7-6a983aeb6bca" />
<img width="600" height="294" alt="image" src="https://github.com/user-attachments/assets/74b6d422-8aef-4a80-897d-527743ba9cb6" />

* K-means

<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/05c7c117-8fd9-4b7a-b978-9fa8e87fac79" />


## 23. 지도
* 지도 데이터없음 이슈
 * 지도 시각화 장점: 공간 데이터가 직관적으로 다가옴
 * 지도 시각화 단점: 구역을 어떻게 나누냐에 따라 해석이 달라짐

## 24. 계산된 필드 
* sum[profit] / sum[sales]랑 [profit] / [sales] 의 값이 왜 다를까
 * sum([Profit]) / sum([Sales])은 매출이 큰 행에 더 많은 가중치를 부여하는 계산입니다. → 즉, 가중 평균
 * 반면 [Profit] / [Sales]는 각 행의 단순 수익률이므로, 단순 평균을 하면 매출이 작든 크든 똑같이 취급됩니다.

* 자주 쓰는 함수
<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/59ba7f02-1fd0-44d6-9b31-344f595c084b" />

## 25. IF 함수
* 집합 또는 T/f 필드 경우 그 자ㅔ로 IF 뒤 조건부분에 사용 가능 

<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/204125c2-c8dd-4a54-920c-54ac2fecdc42" />


## 수강 인증
<img width="357" height="416" alt="image" src="https://github.com/user-attachments/assets/8738c79a-0dea-4b57-a39a-c2554a6d5c78" />

## 느낀점
태블로 기능법은 익힌 것 같음.
대시보드 만들면서 심화 버전 학습해보고 싶다~
