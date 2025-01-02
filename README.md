# 한국어 가짜 구매후기 생성과 탐지 성능 평가

한국어로 생성된 가짜 구매후기 데이터를 공개합니다. <br/>
해당 연구는 지능정보연구 제 30권 2호에 개제되어 있습니다. <br/>
[논문 PDF 다운로드](https://www.jiisonline.org/files/DLA/20240630225137_16.%EA%B0%95%EC%A3%BC%EC%98%81(%EC%B5%9C%EC%A2%85).pdf?PHPSESSID=039313b0723e169a7164eb0416f16b72)



## 데이터
- 생성에는 KULLUM 모델을 활용하였으며, 쿠팡 플랫폼에서 수집된 97,365건의 데이터로 파인튜닝하였습니다. 
- 7가지 품목에 대해 생성하였으며, 총 데이터 개수는 3,542건 입니다.   
- 7가지 품목 별 생성된 텍스트 개수는 다음의 표와 같습니다.
- 파일 위치: './data/generated_revews.csv'


| NO. | 품목 | 개수 |
| --- | --- | --- |
| 1 | 가전디지털 | 500 | 
| 2 | 도서/음반/DVD | 539 |
| 3 | 반려동물용품 | 521 |
| 4 | 스포츠/레저  | 489 |
| 5 | 완구/취미 | 506 |
| 6 | 주방용품  | 494 |
| 7 | 홈인테리어 | 493 |

## 데이터 구성 
생성데이터는 다음의 컬럼으로 구성되어 있습니다. 

| NO. | 컬럼 | 설명 |
| --- | --- | --- |
| 1 | gen_text | 생성된 텍스트 |
| 2 | category | 제품품목 |
| 3 | label  | CG (computer-generated) |


### 인용
해당 GitHub 내의 데이터를 사용할 때는 아래의 인용 문구를 기재해 주시기 바랍니다.

```bibtex
@article{Kor_FakeReviews,
  author = {강주영, 송민},
  title = {한국어 가짜 구매후기 생성과 탐지 성능 평가},
  journal = {지능정보연구},
  issn = {2288-4866},
  year = {2024},
  volume = {30},
  number = {2},
  pages = {313-328}
}
