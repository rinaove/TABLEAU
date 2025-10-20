📌Tableau 정규과제는 매주 정해진 **유튜브 강의를 통해 태블로 이론 및 기능을 학습한 후, 실습 문제를 풀어보며 이해도를 높이는 학습 방식**입니다. 

이번주는 아래의 **Tableau_4th_TIL**에 명시된 유튜브 강의를 먼저 수강해주세요. 학습 중에는 주요 개념을 스스로 정리하고, 이해가 어려운 부분은 강의 자료나 추가 자료를 참고해 보완하세요. 과제 작성이 끝난 이후에는 **Github에 TIL과 실습 인증 결과를 업로드 후, 과제 시트에 제출해주세요.**



**(수행 인증샷은 필수입니다.)** 

> 태블로를 활용하는 과제인 경우, 따로 캡쳐도구를 사용하여 이미지를 첨가해주세요.



## Tableau_4th_TIL

### 39. LOD

### 40. EXCLUDE

### 41. INCLUDE

### 42. 매개변수 

### 43. 매개변수 실습

### 44. 매개변수 실습

### 45. 마크카드

### 46. 서식계층

### 47. 워크시트 



<br>

## 주차별 학습 (Study Schedule)

| 주차  | 공부 범위          | 완료 여부 |
| ----- | ------------------ | --------- |
| 0주차 | **강의 1 ~ 9강**   | ✅         |
| 1주차 | **강의 10 ~ 19강** | ✅         |
| 2주차 | **강의 20 ~ 29강** | ✅         |
| 3주차 | **강의 30 ~ 38강** | ✅         |
| 4주차 | **강의 39 ~ 47강** | ✅         |
| 5주차 | **강의 48 ~ 59강** | 🍽️         |
| 6주차 | **강의 60 ~ 69강** | 🍽️         |

> **🧞‍♀️ 오늘의 스터디는 지니와 함께합니다.**

<!-- 여기까진 그대로 둬 주세요-->



---

# 학습 내용 정리

## 39강. LOD

<!-- INCLUDE, EXCLUDE, FIXED 등 본 강의에서 알게 된 LOD 표현식에 대해 알게 된 점을 적어주세요. -->

<img width="1552" height="917" alt="image" src="https://github.com/user-attachments/assets/2256b731-02bb-45d3-9a29-d6772fa28ca7" /># Tableau 4주차 정규과제


1. FIXED에서 설정한 차원이 기호에 포함되어 있을 때

<img width="1552" height="917" alt="image" src="https://github.com/user-attachments/assets/95025e05-60a4-4a5d-b6ef-39937c4de3a5" />

2. FIXED에서 설정한 차원이 기호에 포함되어 있지 않을 때 (뭔말이지)

<img width="1552" height="917" alt="image" src="https://github.com/user-attachments/assets/cf1d54ac-d997-4a2a-8de9-b3135c1a4b4c" />


## 40. LOD EXCLUDE

<!-- INCLUDE, EXCLUDE, FIXED 등 본 강의에서 알게 된 LOD 표현식에 대해 알게 된 점을 적고, 아래 두 질문에 답해보세요 :) -->

<img width="1552" height="917" alt="image" src="https://github.com/user-attachments/assets/96ab91a4-dd65-4e7b-ade6-e2498f6414dc" />


> **🧞‍♀️ FIXED와 EXCLUDE을 사용하는 경우의 차이가 무엇인가요?**

```
fixed는 현재 뷰와 관련없이 특정 차원만 계산 / exclude는 뷰와 관련있기 때문에 필터 시 값 영향 받음
```

<img width="1552" height="917" alt="image" src="https://github.com/user-attachments/assets/650b2c1a-acee-4730-8ca0-23ac8029af15" />


> **🧞‍♀️ 왜 ATTR 함수를 사용하나요?**

```
ATTR()은 뷰(예: 막대, 원, 셀 등)에서 단일 파티션으로 그룹화되는 기초 데이터의 각 레코드에서 모든 값을 비교하기 위해
```



## 41. LOD INCLUDE

<!-- INCLUDE, EXCLUDE, FIXED 등 본 강의에서 알게 된 LOD 표현식에 대해 알게 된 점을 적고, 아래 두 질문에 답해보세요 :) -->

<img width="1552" height="917" alt="image" src="https://github.com/user-attachments/assets/bfe0fd7a-8ceb-4689-9f3a-a6939df882c8" />


> **🧞‍♀️ 그렇다면 어떤 경우에 각 표현식을 사용하나요? 예시와 함께 적어보아요**


```
뷰에 표시되는 값이 차원이면, fixed lod 표현식만 사용 가능. 차원과 측정값 모두 반환
include와 exclude 표현식들은 측정값만 반환. 반환값이 차원 필터의 영향을 받으면 include, exclude만 사용 가능.
*공부한 것을 바탕으로 제미나이와 함께 소통함*

| 특징 | FIXED | INCLUDE | EXCLUDE |
| :--- | :--- | :--- | :--- |
| **기준 세부 수준** | **지정된 차원에 고정** (뷰 LOD와 무관) | **뷰 LOD +** 지정된 차원 | **뷰 LOD -** 지정된 차원 |
| **필터 영향** (일반 차원 필터) | **무시함** (먼저 계산됨) | **영향받음** (나중에 계산됨) | **영향받음** (나중에 계산됨) |
| **반환 값 유형** | **측정값 (집계)** <br> 또는 **차원 (비집계)** | **측정값 (집계)만** | **측정값 (집계)만** |
| **주요 용도** | 뷰와 상관없는 전체 기준값 (예: 전체 평균) | 뷰보다 *더* 세분화된 계산 | 뷰보다 *덜* 세분화된 계산 (예: % of Total) |

```



## 42. 매개변수

<!-- 매개변수에 대해 알게 된 점을 적어주세요 -->

```
매개변수는 반드시 계산서, 필터, 참조선을 함께 사용해야 함
```

<img width="1552" height="917" alt="image" src="https://github.com/user-attachments/assets/6150c9ac-40b9-4241-829d-4aea1ea724b9" />


> **🧞‍♀️ 집합에도 매개변수를 적용할 수 있나요? 시도해봅시다**

<img width="1552" height="917" alt="image" src="https://github.com/user-attachments/assets/b33fe844-3c97-482c-85bd-c0605c086bfe" />




## 43. 매개변수 실습

<!-- 영상 묶음에 포함되지 않아 찾기 어려우실까 링크를 아래에 첨부하겠습니다. 수강 후 삭제해주세요-->

(맥에서 매개변수 수정하려니까 계속 튕겨서 #43은 실습 없이 수강 인증하겠습니다.)

<img width="1552" height="917" alt="image" src="https://github.com/user-attachments/assets/da7877a4-6eaf-46ac-b50d-f5c65a047ec8" />

<img width="1552" height="917" alt="image" src="https://github.com/user-attachments/assets/f0a73409-23b7-43a1-8e9b-c0e4cf431195" />


## 44. 매개변수 실습

<!-- 매개변수에 대해 알게 된 점을 적어주세요 -->

<img width="1552" height="917" alt="image" src="https://github.com/user-attachments/assets/fc603972-d345-4bed-9770-462101b5dd6b" />

<img width="1552" height="917" alt="image" src="https://github.com/user-attachments/assets/5333d984-96b9-44c3-b254-b7124411f14a" />

<img width="1552" height="917" alt="image" src="https://github.com/user-attachments/assets/06da82a9-3342-419a-b7e5-18080583d4bb" />


## 45. 워크시트 마크카드

<!-- 마크카드에 대해 알게 된 점을 적어주세요 -->

```
워크시트에서 차트 만들 시 해당 시트에 있는 데이터를 마크라고 함. 마크 서식을 변경하기 위해 마크카드를 사용해야 함.
마크 값 변경 시 차트는 유지되면서 마크 값이 변경됨.
```

<img width="172" height="234" alt="image" src="https://github.com/user-attachments/assets/d9f693ef-1a89-4478-b1ce-7f4588bafd86" />

<img width="930" height="431" alt="image" src="https://github.com/user-attachments/assets/b877ad31-c82d-4096-9643-78c54f647d2c" />

<img width="686" height="428" alt="image" src="https://github.com/user-attachments/assets/14af0209-b44b-450b-a295-a794ed61472e" />

<img width="1552" height="917" alt="image" src="https://github.com/user-attachments/assets/a5706bcc-16bb-424a-a802-9df1aaea3f03" />


## 46. 서식 계층

<!-- 서식계층에 대해 알게 된 점을 적어주세요 -->

<img width="1552" height="917" alt="image" src="https://github.com/user-attachments/assets/6781d5ea-7018-41da-8969-c1aa5f85d8d1" />


> **🧞‍♀️ 서식계층을 일반적인 것에서 구체적인 것 순서로 기입해보세요**

```
워크 시트 서식 > 행/열 서식 > 특정 필드 > 필드 레이블 > 도구설명 / 제목 / 마크
```



## 47. 워크시트 서식

<!-- 워크시트 서식에 대해 알게 된 점을 적어주세요!-->

<img width="1552" height="917" alt="image" src="https://github.com/user-attachments/assets/33437e1c-a06f-4ff6-89c3-756611933cd6" />


# 확인문제

## 문제 1.

```
가장 많이 주문한 사람들은 물건 배송을 빨리 받았을까요?
조건을 준수하여 아래 이미지를 만들어봆시다.
1) 국가/지역별(이하 '나라'로 통칭), 범주별로 배송일자가 다를 수 있으니 먼저, 나라별/범주별로 평균 배송일자를 설정한 뒤,
2) 각 나라에서 가장 많이 주문한 사람의 이름을 첫 번째 열,
3) 그 사람이 주문한 제품 이름을 2번째 열,
4) 각 상품이 배송까지 걸린 날 수를 표현하고
5) 그리고 만약 배송이 각 나라/범주별 평균보다 빨랐다면 '빠름', 같다면 '평균', 느리다면 '느림' 으로 print 해주세요. 
```

![alt text](images/Week4-1.png)



<!-- 여기까지 오는 과정 중 알게 된 점을 기입하고, 결과는 시트 명을 본인 이름으로 바꾸어 표시해주세요.-->



## 문제 2.

```
채원이는 태블로를 쓰실 수 없는 상사분께 보고하기 위한 대시보드를 만들고 싶어요. 

제품 중분류별로 구분하되 매개변수로써 수익, 매출, 수량을 입력하면 저절로 각각 지표에 해당하는 그래프로 바뀌도록 설계하고자 해요.

 어떤 값이 각 지표의 평균보다 낮은 값을 갖고 있다면 색깔을 주황색으로, 그것보다 높다면 파란색으로 표시하고 싶어요. 그 평균값은 각 지표별로 달라야 해요.
```

![alt text](images/Week4-2.png)



<!-- 예시 사진은 지워주세요-->



<br>

<br>

### 🎉 수고하셨습니다.
