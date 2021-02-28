This is a project to create a web page that lists current real-time issues (topics) about things happening in Korea by ranking.

## 한국에서 발생하는 일들에 대한 현재 실시간 이슈(토픽)을 집계하여, 순위별로 나열된 웹페이지를 만드는 프로젝트입니다.
---
글 읽는 순서
1. 이 repository의 readme 파일
2. github.io의 글 https://baekjongseong.github.io/news_crawl/
3. repository 핵심 파일들 추후 업데이트 
---
프로젝트 핵심은 다음과 같습니다 
기존 Naver 실시간 검색어 서비스 폐지(2021.02.25)에 따른 불편함을 해소해보고자 직접 구현한 실시간 토픽 서비스

|구분|Naver|My project|
|---|---|---|
|카테고리|통합형|스포츠 & 연예계 & 정치사회 & 금융.주식/코인(예정)|
|갯수|20개|각 카테고리별 20개 (총 4개의 카테고리)|
|근거|네이버 포털 사이트 누적 검색 횟수|네이버 뉴스(각 카테고리별 상위 뉴스들의 핵심어를 추출하여 순위로 등재)|
|방식|자체 집계 가능|포털사이트 request를 통한 응답으로 해당 페이지(랭킹 뉴스) 크롤링을 통하여 순위로 등재|
|목적|-|상업용 X, 오로지 프로젝트용|
---

+ page1 = 카테고리
	+ 주식종목 & 금융 20개 (네이버금융 많이본 + 장중특징주 + 주요뉴스)
	+ 영화드라마 & 연예인 20개 (네이버연예뉴스)
	+ 스포츠 20 개 (종목별 네이버 스포츠 뉴스)
	+ 경제 & 정치 & 사회 20개 (네이버뉴스)

+ page 2
  + 데이터랩 같은 지표형식
  + 사람들이 납득할 수 있게 이슈별로 그래프 하나씩 추가
 
+ 진행방식
  + 랭킹 차트(조회수 / comment 수를 통해 시작)

![2021-02-27-naver_news](https://user-images.githubusercontent.com/79182947/109386605-0cd33180-793f-11eb-857c-23aba6b74003.png)
