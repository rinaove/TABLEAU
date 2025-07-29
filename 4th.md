# 🎨 태블로 4주차
- 이번주 목표
- [ ] 1시간 강의 다 듣기
- [ ] 태블로 vs 엑셀
- [ ] c
- [ ] Data investigation in 태블로


 ## 19. Level of Detail
 > 1) 태블로 vs 엑셀
* 태블로: 데이터 시각화 도구 vs 엑셀: 데이터 원본 그 자체 (스프레드시트)
  * 데이터 탐색 목적이 quick summary라면 태블로가 강점
1) 엑셀은 표 중심 / 태블로는 그래프 중심
2) 엑셀은 원본 수정 가능 / 태블로는 원본 수정 불가
3) 엑셀은 측정값을 있는 그대로 보여줌 / 태블로는 측정값을 집계해서 보여줌

 > 2) Aggregation in 태블로
<img width="757" height="281" alt="image" src="https://github.com/user-attachments/assets/704f53b8-87af-4342-aa8c-82bcffa6239b" />

* 엑셀은 필요에 따라 sum(), sumif() 함수로 측정값을 집계하지만, 태블로는 측정값 집계를 default로 보여줌
* 태블로는 어떻게 집계값을 나눌지(slice)에 대한 고민을 충분히 해야 함. 또한, slice한 데이터가 어떤 뜻일지도 이해해야 함

> 3) Data investigation in 태블로
* 데이터셋은 몇 개 행, 열로 구성되어 있는지
* 각 행이 의미하는 바는 무엇일지
* 단 하나의 필드로 데이터셋 디테일까지 최종 분기 가능
* 몇 개의 필드를 조합하여 데이터셋 디테일까지 분기 가능
* 어떤 필드를 조합하더라도 데이터셋의 디테일까지 분기 불가능한 경우
  * 뻥튀기 되는 데이터 조심 (합계값으로 default가 설정되기에)
  * App이 아닌 Review per App으로 조합하기
  * { Fixed [App]: MAX([Reviews]) }
 ## 수강 인증
<img width="363" height="265" alt="image" src="https://github.com/user-attachments/assets/bd9b739e-a4df-4bff-b4bb-4cf0ea51ebd2" />

 ## 느낀점
 귀로는 이해했으나 손으로 입력하기는 어려운 태블로... 실습 한번 해봐야 내가 정신차릴듯
