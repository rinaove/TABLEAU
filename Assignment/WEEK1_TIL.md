# Tableau 2주차 정규과제

📌Tableau 정규과제는 매주 정해진 **유튜브 강의를 통해 태블로 이론 및 기능을 학습한 후, 실습 문제를 풀어보며 이해도를 높이는 학습 방식**입니다. 

이번주는 아래의 **Tableau_2nd_TIL**에 명시된 유튜브 강의를 먼저 수강해주세요. 학습 중에는 주요 개념을 스스로 정리하고, 이해가 어려운 부분은 강의 자료나 추가 자료를 참고해 보완하세요. 과제 작성이 끝난 이후에는 **Github에 TIL과 실습 인증 결과를 업로드 후, 과제 시트에 제출해주세요.**



**(수행 인증샷은 필수입니다.)** 

> 태블로를 활용하는 과제인 경우, 따로 캡쳐도구를 사용하여 이미지를 첨가해주세요.



## Tableau_2nd_TIL

### 10. 차원과 측정값

### 11. 시각화

### 12. 막대 그래프

### 13. 누적막대 그래프

### 14. 병렬막대 그래프

### 15. 누적병렬막대 그래프

### 16. 라인 그래프

### 17. 맵 작성

### 18. 텍스트 레이블

### 19. 트리맵과 하이라이트 테이블



<br>

## 주차별 학습 (Study Schedule)

| 주차  | 공부 범위          | 완료 여부 |
| ----- | ------------------ | --------- |
| 1주차 | **강의 1 ~ 9강**   | ✅         |
| 2주차 | **강의 10 ~ 19강** | ✅         |
| 3주차 | **강의 20 ~ 29강** | 🍽️         |
| 4주차 | **강의 30 ~ 39강** | 🍽️         |
| 5주차 | **강의 40 ~ 49강** | 🍽️         |
| 6주차 | **강의 50 ~ 59강** | 🍽️         |
| 7주차 | **강의 60 ~ 69강** | 🍽️         |

<!-- 여기까진 그대로 둬 주세요-->



---

# 1️⃣ 학습 내용 정리

## 10강: 차원과 측정값

<!-- 차원과 측정값에 관해 배우게 된 점을 적어주세요 -->

> **🧞‍♀️ 차원과 측정값의 고유한 특성에 대해 설명해주세요.**

```
테이블 2가지 영역이 나타남.
데이터 유형에 따라 필드를 차원 또는 측정값으로 할당
차원: 정성적 값, 독립적 값을 지닌 필드 (집계X, 불연속적)
측정값: 정량적 값, 차원의 세부 항목 (집계O, 연속적)```
```
*Quiz: 차원은 불연속형이고, 측정값은 연속형이다 (o, **x**)
```
정답: X
차원은 기본적으로 불연속형,
측정값은 기본적으로 연속형이지만, 상황에 따라 사용자가 바꿀 수 있다.
```


## 11강: 시각화

<!-- 시각화 관해 배우게 된 점을 적어주세요 -->
```
차원은 대부분 불연속형이며, 표 형태로 시각화했을 때 머리글 표시됨
측정값은 대부분 연속값, 표 형태로 시각화했을 때 패널로 표시됨
```

<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/3bd7845f-5493-4838-b7c5-987d6d9bde31" />


*Quiz: 차원은 대부분 불연속형이며 표 형태로 시각화했을 때 머리글로 표시되고, 측정값은 대부분 연속형이므로 표 형태로 시각화 진행했을 때 패널로 추가된다.(**o**, x)*
```
정답: O
```


## 12강: 막대그래프

<!-- 막대그래프에 관해 배우게 된 점을 적어주세요 -->
```
내림차순 정렬 시 필드 우클릭 후 정렬을 수동으로 지정가능
```

<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/b10f7e7a-cce4-4938-a027-04a6572f5044" />



## 13강: 누적막대그래프

<!-- 누적막대그래프에 관해 배우게 된 점을 적어주세요 -->
```
세부 정보에 컬럼 넣으면 세부 그래프 값으로 볼 수 있음
테이블(아래로, Down) → 같은 열 안에서 위→아래로 누적
테이블(옆으로, Across) → 같은 행 안에서 좌→우로 누적
```

<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/2cdaedd5-8d5b-4b12-ac41-649ea4cab96f" />


<!-- 테이블(아래로)와 테이블(옆으로)의 계산 방식을 습득해보세요. 이에 관련해 아래 참고자료도 있습니다 :) -->

<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/366f9e37-9c5b-42ac-8641-45792fba9af9" />



## 14강: 병렬막대그래프

<!-- 병렬막대그래프에 관해 배우게 된 점을 적어주세요 -->
```
불연속형 필드를 연속형 필드로 변경 시 시간의 흐름 인지함
```

![alt text](https://raw.githubusercontent.com/DArt-B-Official/Tableau_Template/main/images/Week1-1.png)

<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/4bd11d71-6847-404a-ac2f-af0074d40924" />



> *🧞‍♀️ 끊어진 색상으로 배치되어 표현되는 경우와 이어지는 그라데이션 색으로 표현되는 경우 두 가지가 있습니다. 위 사진의 경우 왜 색깔이 끊어지는 색상으로 표시되지 않고 그라데이션으로 표시되었나요? 데이터의 특성과 관련하여 이야기해 봅시다.*

```
여기에 답을 적어주세요!
```



## 15강: 누적병렬막대그래프

<!-- 누적병렬막대그래프에 관해 배우게 된 점을 적어주세요 -->
```
연도는 연속/불연속형 그래프 비슷
월은 연속형 변경 -> 연도별 월 표시 / 불연속형 변경 -> 연도누적 월 표시
```
<img width="1552" height="923" alt="스크린샷 2025-09-12 오후 11 54 47" src="https://github.com/user-attachments/assets/a998dfef-1f21-4d66-8ce3-22ad9df7b4ff" />

<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/1f24155b-4e4f-46d4-9400-1ad5bf11a80c" />



![alt text](https://raw.githubusercontent.com/DArt-B-Official/Tableau_Template/main/images/Week1-2.png)




> *🧞‍♀️ 위 사진에서는 Profit과 Sales를 측정값으로 두었습니다.  개별 칼럼(태블로에서는 #필드라 명칭합니다)을 열/행에 두는 대신, '측정값'을 사용하고 측정값 선반에 필드를 올려둡니다. 이런 방식을 사용하는 이유가 무엇일지, 어떻게 사용할 수 있을지 고민해보세요*

```
측정값을 쓰면 여러 숫자 지표를 한 차트에서 비교하거나, 사용자가 선택해서 볼 수 있게 만들 수 있음
```

<!-- 정답은 없습니다 -->



## 16강: 라인그래프

<!-- 라인그래프에 관해 배우게 된 점을 적어주세요 -->


<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/f0ecec47-3379-4776-b9a5-90c9093279a0" />

<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/1fe1e782-994e-4198-8a34-58086c0acf6a" />


## 17강: 맵작성

<!-- 맵차트 관해 배우게 된 점을 적어주세요 -->

```
지구본 클릭 > 지리적 역할 > 필드의 각 값을 위도와 경도에 연결함
맵차트에서도 이중축 설정 가능
마크 계층 추가에 도시 필드 드래그 시 > 도시와 주를 표시하는 마크 창이 생김
```

<img width="884" height="421" alt="image" src="https://github.com/user-attachments/assets/5b9e66f0-55ec-4a03-9b1f-caa4be0f3366" />


```js
## 참고
Country/Region - 나라/지역
State/Province - 시/도
City - 시
County - 군
Postal Code - 우편번호
Area Code - 지역 코드
Airport - 공항
MSA/CBSA (Metropolitan Statistical Area) - 광역 통계 지역
Longitude - 경도
Latitude - 위도
```



## 18강: 텍스트테이블

<!-- 텍스트테이블에 관해 배우게 된 점을 적어주세요-->
```
텍스트 테이블은 데이터를 표 형태로 보여주는 가장 기본적인 시각화 방식으로, 차원은 행/열 머리글로, 측정값은 셀 안에 숫자로 표시된다.
주로 수치 비교, 데이터 점검, 단순 요약에 활용되며 시각적 인사이트보다는 정량적 확인에 적합하다.
```

<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/27c6c198-dcff-4688-92fe-6fe3f2341add" />



## 19강: 트리맵과 하이라이트테이블

> *🧞‍♀️하이라이트 테이블 등에서 두개 이상의 측정값을 사용하는 경우, 함께 색을 표현하게 되면 단위가 달라 정확한 값을 표현할 수 없습니다. 이때 클릭해야 하는 항목은?*

```
마크의 측정값 마우스 우클릭 > 별도의 범례사용 클릭 
```

<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/0b0da7ec-16ac-4b8a-8e43-f87898d10003" />
<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/b1a435f5-8d77-4e06-ac25-bc4da44cb04d" />

<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/4e8d89d3-91b4-4d66-a025-7567742f66b7" />

<br>

# 2️⃣ 확인문제

## 문제1

```js
지민이는 superstore의 한국 수출 관리 업무를 맡고 있습니다. 국가/지역이 우리나라, 즉 'South Korea'인 데이터만을 필터링하여, 상품 하위범주 별로 각 하위범주가 매출의 비율 중 얼마만큼을 차지하는지를 트리맵으로 확인하고 싶습니다. 트리맵의 각 네모 안에 표시되는 텍스트에는 **해당 범주의 이름과 전체에서 해당 범주가 차지하는 비율**이 표시되었으면 합니다.

지민이를 도와주세요! (풀이를 찾아가는 과정을 기술해주세요)
```

```
필터에 국가/지역 드래그 > South Korea 설정 > 하위 범주를 레이블로 드래그 > 합계(매출)을 색상, 크기, 레이블 드래그 > 합계(매출) 우클릭 후 퀵 테이블 계산 > 구성 비율 클릭
```
<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/3915b755-3fb6-4f88-9f74-ae57423766ee" />



## 문제2

```js
주현이는 국가/지역별로 매출과 수익의 증감을 시간에 흐름에 따라 표현하고자 합니다. 특히 **한국/중국/일본**을 비교하고자 해당 3국을 남기고 필터링했고, 3개 국가를 매출과 수익이라는 두 가지 지표로 확인해보았습니다.

아래는 위 설명을 표현해본 예시입니다.
```


![alt text](https://raw.githubusercontent.com/DArt-B-Official/Tableau_Template/main/images/Week1-3.png)


```js
레퍼런스와 꼭 같지 않아도 자유롭게 표현하고, 그 과정을 기술해주세요.
```

```
국가/지역 아시아 3국 필터링 > 월 주문 날짜 (열) 삽입 후 연속형 데이터로 변경 > 합계(매출) 및 합계(수익 (행) 삽입 후 이중축 설정 > 축 동기화 설정 후 축 제목 '배송 날짜의 월' 변경 > 색상 변경
```
<img width="1552" height="923" alt="image" src="https://github.com/user-attachments/assets/fa9ef9e1-68a4-4249-9bcc-a9cf2f1197f3" />




### 참고 자료

```js
테이블 계산에서 '다음을 사용하여 계산'에는 테이블 당 계산과 패널 당 계산이 있습니다. 이에 대해 이해하는 것이 꼭 필요하기 때문에, 외부 레퍼런스를 참고하여 이 단계에서 꼭! 학습 후, 넘어가주세요 :)
```



![테이블계산](https://velog.velcdn.com/images/eunsuh/post/8a56ab15-930d-4ad6-b5ab-74513863115f/image.png
)



[참고 외부자료 링크는여기를클릭하십시다](https://velog.io/@eunsuh/Tableau-%EB%A0%88%EB%B2%A8UP-%EA%B0%95%EC%9D%98-%EC%A0%95%EB%A6%AC-1-%ED%85%8C%EC%9D%B4%EB%B8%94-%EA%B3%84%EC%82%B0)

<br>

<br>

### 🎉 수고하셨습니다.
