# 국민대·정릉시장 맛집 토픽 모델링

[![Python](https://img.shields.io/badge/python-3.10-3776AB?logo=python&logoColor=white)](https://www.python.org) [![License](https://img.shields.io/badge/license-Apache--2.0-blue.svg)](LICENSE)

국민대학교 텍스트 데이터 분석 수업에서 국민대·정릉시장 주변 맛집 리뷰를 수집하고 LSA/LDA 토픽 모델링을 수행한 개인 프로젝트입니다. 크롤링과 전처리를 다룬 중간 과제(Part-01)와 토픽 모델링을 다룬 기말 과제(Part-02)로 이어집니다.

## 개요

| 구분 | 내용 |
| --- | --- |
| 수업 | 국민대학교 텍스트 데이터 분석 |
| 기간 | 2022.09 – 2022.12 |
| 형태 | 개인 프로젝트 |
| 데이터 | 네이버 VIEW, 다이닝코드, 망고플레이트, 서울시 성북구 공공데이터 |
| 분석 | Selenium 크롤링, KoNLPy 형태소 분석, LSA, LDA |

## 접근

- 네이버 VIEW, 다이닝코드, 망고플레이트에서 리뷰를 수집하고, 서울시 성북구 일반음식점 인허가 정보를 함께 활용했습니다.
- Selenium으로 동적 페이지를 크롤링하고 BeautifulSoup을 보조로 썼습니다.
- Komoran·Hannanum·Kkma·Twitter(Okt)·Mecab 형태소 분석 결과를 비교했습니다.
- 불용어와 빈도 기준으로 걸러낸 뒤 LSA와 LDA로 토픽을 추출했습니다.
- 토픽별 키워드와 음식점을 매핑해 시각화했습니다.

## 저장소 구성

제출 당시의 파일명(Part-01 중간 · Part-02 기말)을 그대로 남겼습니다.

```text
.
├── notebooks/
│   ├── Web_crawling+LSA,LDA-Part-01.ipynb   # 중간: 리뷰 크롤링과 전처리
│   └── Web_crawling+LSA,LDA-Part-02.ipynb   # 기말: LSA·LDA 토픽 모델링
├── reports/
│   ├── Web_crawling+LSA,LDA-Part-01.pdf      # 중간 노트북 실행본
│   ├── Web_crawling+LSA,LDA-Part-02.pdf      # 기말 노트북 실행본
│   └── Web_crawling+LSA,LDA-Part-02.mp4      # 기말 발표 영상
├── requirements.txt
└── README.md
```

## 공개 범위

- 크롤링한 리뷰 원본과 불용어 파일, 중간 산출물은 포함하지 않았습니다. 대신 노트북을 실행한 결과를 PDF와 발표 영상으로 남겼습니다.
- 노트북 출력은 리뷰 원문이 담겨 있어 비웠고, 실행 결과는 함께 둔 PDF에서 확인할 수 있습니다.
- 코랩 드라이브 절대경로는 `data/` 기준으로 정리했습니다.

## 라이선스

Apache License 2.0. 자세한 내용은 [LICENSE](LICENSE)에 있습니다.
