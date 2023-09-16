# 파이썬 투자 포트폴리오 만들기

## 개요: 퀀트란 무엇인가?

**퀀트(Quant): 모형을 기반으로 금융 상품의 가격을 산정하거나, 이를 바탕으로 투자하는 사람**
- 퀀트 투자는 규칙에 가빈하기에 객관성이 높음
- 데이터와 규칙만 있다면 한 번에 수백, 수천 종목에 대한 분석도 가능
- 규칙에 기반하므로 감정에 휘둘릴 위험이 낮음
- 동일한 규칙을 누구든지 반복할 수 있음
- 규칙을 철저하게 지킬 경우 위험 통제 능력이 높음

### 1. 데이터

**데이터: 가장 기본이 되면서 중요한 밑천**
- 데이터가 부실하거나 틀린 내용이라면 잘못된 전략을 만들어 손실을 보게 될 것
- 데이터가 다채롭다면, 이를 다루는 퀀트의 실력에 따라 얼마든지 다양한 전략을 만들 수 있음

**주요 데이터 수집처**
- ClariFi
- Capital IQ
- FactSet
- Thomson Reuters
- Bloomberg

**웹 스크래핑(Web Scraping)&크롤링(Crawling)**
- 클로링과 API를 활용해 국내 및 글로벌 데이터 수집 가능

### 2. 프로그래밍

**데이터 클렌징(Data Cleansing)**
- 엑셀은 응용성 및 효율성 측면에서 프로그래밍에 비해 매우 비효율적
- 종목 수가 수천 종목을 넘어간다면, 데이터를 손으로 일일이 처리하는 것이 사실상 불가능
- 단순 반복 작업은 프로그래밍이 훨씬 효율적

**백테스트(Backtest)**
- 엑셀에선 12개월 -> 6개월 누적 수익률 테스트 변경을 위해 반복적인 수식 변경 및 드래그 작업 필요
- 프로그래밍 이용 시 n = 12 -> n = 6 수정만 해주면 됨
- 또한 엑셀에서 새로운 전략 백테스트 시, 해당 데이터를 새로운 엑셀 파일에 복사해 작업한 후 다시 저장해야 함
- 만일 데이터가 바뀔 경우 다시 여러개 엑셀 시트의 데이터를 일일이 바꿔야 함
- 물론 하나의 엑셀 파일 내에서 모두 작업할 수 있지만, 이 경우 속도가 상당히 저하되는 문제 발생
- 프로그래밍 이용 시 각 전략 별 스크립트 파일만 작성해주면 됨. 데이터 변경 시에도 원본 데이터 하나만 수정

### 3. 파이썬(Pyhton)

**파이썬: 가장 대중적인 프로그래밍 언어**

### 4.SQL

**데이터베이스(DataBase, DB)**
- 여러 사람이 공유하여 사용할 목적으로 체계화하여 통합, 관리하는 데이터의 집합
- 티커(Ticker), 주가, 재무제표, 모굪 주가 등 투자와 관련된 모든 데이터를 DB에 저장 후 관리 및 사용

**DBMS(DataBase Management System)**
- 다수의 사용자들이 DB 내의 데이터에 접근할 수 있또록 해주는 SW 도구 집합
- 관계형 데이터베이스(Relational DB): 엑셀 시트철머 열과 행으로 이루어진 2차원 테이블 형식

**SQL(Structured Query Language): DB 데이터 처리 전용 언어**

## 목차

1. 파이썬 복습
2. 데이터 분석 복습
3. SQL 복습
4. 크롤링
5. DB구성
6. 전략 구성
7. 백테스트
8. KIS Developers 연결
9. 실전 투자
10. 트레이딩 봇 개발
11. 수익
12. 리밸런싱