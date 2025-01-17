# 🚌 여행 트렌드 분석 파이프라인 구축 프로젝트 🚗
## 프로젝트 개요

### 목표

- 여행 로그 데이터를 기반으로 트렌드 분석 파이프라인을 구축하고 자동화하여 새로운 데이터라고 가정한 주차별 데이터를 배치로 실행한다.
- 여행 데이터를 분석하여 지역별 방문 빈도, 활동 유형, 소비 패턴 등의 인사이트를 제공한다.
- 대시보드 시각화를 통해 국내 여행의 전반적인 트렌드를 쉽게 파악한다.

### 핵심 분석 내용

1. 지역별 방문 빈도 분석
2. 활동 유형 및 소비 금액 분포 분석
3. 이동 경로 시각화
4. 여행 비용–만족도 상관관계 분석
5. 버블 차트를 활용한 소비–방문수 시각화

## 아키텍처

### 다이어그램
![데엔싱파티_아키텍처](https://github.com/user-attachments/assets/74afb307-6703-4cfc-b8ce-02c0b8121b1c)

### 구성요소
- 원본 데이터 저장: AWS S3
- 데이터 처리: Apache Spark, Python
- 워크플로 관리: Apache Airflow
- 데이터 웨어하우스: AWS Snowflake
- 데이터 시각화: Preset

## 구현 내용

1. 데이터 준비 및 ETL
    - Spark: 대량 데이터 클렌징 및 변환 작업
    - Airflow: 배치 데이터 처리 자동화

2. 데이터 웨어하우스
    - Snowflake: 시간별, 지역별, 활동 유형별 조회 가능한 스키마 설계

3. 시각화
    - Preset: 여행지 지역별 방문 빈도 및 소비 패턴 대시보드

<!-- ## 목표 결과 및 인사이트 -->

<!-- 지역별 방문 분석, 소비 패턴 분석, 이동 경로: 이동 경로 시각화를 통해 주요 방문 지역 간 연결성을 파악-->
