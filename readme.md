

# 1. 배열
## 연습문제
    * 나선형 출력
    * 틱택토 게임
    * 길찾기 게임
    * 행렬회전 
# 2. 재귀
## 재귀 소개
## 재귀의 규칙
    * 기저 조건
    * 분할 정복 방식
    * 예: 피보나치 수열
    * 피보나치 수열: 꼬리 재귀
    * 파스칼의 삼각형
## 재귀의 빅오 분석
    * 점화식
    * 마스터 정리
## 재귀 호출 스택 메모리 

# 3. 집합
## 집합 소개 
## 집합 연산
    * 삽입
    * 삭제
    * 포함

## 기타 유틸리티 합수 
    * 교집합
    * 상위 집합 여부 확인
    * 합집합
    * 차집합

# 4. 검색과 정렬
  ## 4.1 검색
    * 선형 검색
    * 이진 검색
  ## 4.2 정렬
    * 거품 정렬
    * 선택 정렬
    * 삽입 정렬
    * 빠른 정렬
    * 빠른 선택
    * 병합정렬
    * 계수정렬
    * 힙 정렬
    * 자바스크립트 내장정렬
  
# 5. 해시테이블
## 해싱기법
    * 소수 해싱
    * 탐사
    * 재해싱/이중 해싱

## 해시테이블 구현
    * 선형 탐사 사용하기 
    * 이차 탐사 사용하기 
    * 선형 탐사를 활용해 이중 해싱 사용하기 

# 6. 스택과 큐
## 스택
    * 삽입
    * 삭제
    * 접근
    * 검색

## 큐
    * 삽입
    * 삭제
    * 접근
    * 검색

# 7. 연결리스트
## 단일 연결 리스트
    * 삽입
    * 값에 의한 삭제
    * 헤드 항목 삭제

## 이중 연결 리스트
    * 헤드에 항목 삽입하기 
    * 테일에 항목 삽입하기 
    * 헤드의 항목 삭제하기
    * 테일의 항목 삭제하기


# 8. 캐싱
## 캐싱이란? 
## LFU 캐싱
## LRU 캐싱

# 9. 트리
## 일반적인 트리구조
## 이진 트리
## 트리 순회
      * 선순위 순회
      * 중순위 순회
      * 후순위 순회
      * 단계순위 순회
      * 트리 순회 요약

## 이진 검색 트리 
      * 삽입
      * 삭제
      * 검색

## AVL 트리 
      * 단일회전
      * 오른쪽회전
      * 이중회전
      * 트리균형잡기
      * 삽입
      * AVL 트리 예제 종합

# 10. 힙
## 힙에대한 이해
      * 최대 힙
      * 최소 힙

## 이진힙 배열 인덱스 구조
      * 삼투: 위로 아래로 이동
      * 삼투구현하기 
      * 최대 힙예

## 최소 힙 구현완성
## 최대 힙 구현완성
## 힙정렬
      * 오름차순 정렬(최소 힙)
      * 내림차순 정렬(최대 힙)

# 11. 그래프 
## 그래프 기본

## 무지향성 그래프 
      * 간선과 정점 추가하기 
      * 간선과 정점 삭제하기 

## 지향성 그래프 
## 그래프 순회
      * 너비 우선 검색
      * 깊이 우선 검색

## 가중치가 있는 그래프와 최단 경로
      * 가중치가 있는 간선을 지닌 그래프
      * 다익스트라의 알고리즘: 최단경로

# 12. 동적프로그래밍
## 동적 프로그래밍의 필요성
## 동적 프로그래밍의 규칙
      * 중복 부분 문제
      * 최적 부분 구조
      * 예: 걸음 수를 채우는 방법

## 대표적인 동적 프로그래밍 예
      * 패낭 문제 알고리즘
      * 최장 공통 부분 수열 알고리즘
      * 동전 교환 알고리즘
      * 편집 거리 알고리즘



---
# webpack 설정
- js만 함

```
npm init y 
```

```
npm i -D webpack webpack-cli
```

* package.json 설정
```
"build": "webpack",
```

* webpack.confing.js 설정

```
const path = require("path");

module.exports = {
  mode: 'development',
  entry: {
    main: './src/app.js'
  },
  output: {
    path: path.resolve('./dist'),
    filename: '[name].js',
  }
}
```


# lint, prettier
* npm i eslint