# Python 학습 일지 (Study Log)

파이썬 기초 문법 및 활용법을 단계별로 학습하며 정리한 기록입니다.

## 📅 1. 학습 목차 및 내용 SUMMARY
| 순서 | 주제 | 파일명 (.ipynb) | 주요 학습 내용 |
| :--- | :--- | :--- | :--- |
| 01 | 변수 & 문자열 | `ex01_변수, 문자열.ipynb` | • 변수 선언 및 메모리 개념<br>• 문자열 인덱싱 & 슬라이싱<br>• 문자열 포맷팅 (f-string) 및 주요 메서드 |
| 02 | 연산자 | `ex02_연산자.ipynb` | • 산술, 대입, 비교, 논리 연산자<br>• 연산자 우선순위 및 활용 |
| 03 | 조건문 | `ex03_조건문.ipynb` | • if, elif, else 제어문 구조<br>• 조건 판단식 작성 및 중첩 조건문 |
| 04 | 리스트 & 튜플 | `ex04_리스트, 튜플.ipynb` | • 리스트/튜플 생성, 수정, 삭제<br>• 요솟값 추가, 정렬 등의 메서드<br>• Mutability(가변성) vs Immutability(불변성) |
| 05 | 반복문 | `ex05_반복문.ipynb` | • for 문과 while 문 활용<br>• range() 함수 및 리스트 내포 (List Comprehension)<br>• break, continue 흐름 제어 |
| 06 | 딕셔너리 | `ex06_딕셔너리.ipynb` | • Key-Value 구조의 데이터 관리<br>• keys(), values(), items() 활용 |
| 07 | 함수 | `ex07_함수.ipynb` | • 사용자 정의 함수 (def) 및 반환값 (return)<br>• 매개변수 (`*args`, `**kwargs`) 및 Lambda 표현식 |

## 💡 주요 개념 정리
1. **변수와 문자열**
   - **변수:** 데이터를 저장하는 메모리 공간의 이름
   - **문자열 슬라이싱:** `string[start:end:step]` 구문을 통한 부분 문자열 추출
2. **연산자**
   - **산술 연산자:** `+`, `-`, `*`, `/`, `//` (몫), `%` (나머지), `**` (거듭제곱)
   - **논리 연산자:** `and`, `or`, `not`
3. **조건문**
   - 조건에 따라 프로그램 실행 흐름을 제어 (`if - elif - else`)
4. **리스트 vs 튜플**
   - **리스트 (`[]`):** 요소를 자유롭게 추가/수정/삭제 가능 (Mutable)
   - **튜플 (`()`):** 한번 생성되면 요소를 변경할 수 없음 (Immutable)
5. **반복문**
   - **for 문:** 정해진 횟수나 순회 가능한(Iterable) 객체를 순차적으로 반복
   - **while 문:** 조건식이 True인 동안 지속적으로 반복 실행
6. **딕셔너리**
   - **딕셔너리 (`{key: value}`):** Key와 Value의 쌍으로 구성된 데이터 구조이며, Key를 통해 빠르게 값에 접근 가능 (Key 중복 불가)
7. **함수**
   - **사용자 정의 함수 (`def`):** 코드의 재사용성을 높이기 위해 특정 기능을 수행하는 코드 블록을 정의
   - **매개변수 (`*args`, `**kwargs`):** 가변 인수를 받아 다양한 개수의 데이터를 처리 가능
   - **람다 표현식 (`lambda`):** 이름 없는 익명 함수를 간결하게 한 줄로 작성할 때 사용

## 📊 2. 주요 데이터 구조 비교 (Data Structures)
- 🟢 **리스트 (list):** `[1, 2, 3]` — 순서 O, 중복 O, 수정 가능 (Mutable)
- 🔴 **튜플 (tuple):** `(1, 2, 3)` — 순서 O, 중복 O, 수정 불가 (Immutable)
- 🟡 **딕셔너리 (dict):** `{"key": "value"}` — Key-Value 쌍, Key 중복 불가

---

# 파이썬 라이브러리 학습 일지 (NumPy & Pandas)

고성능 다차원 배열 연산 및 수치 데이터 분석 라이브러리인 NumPy와, 표 형태의 데이터를 직관적이고 효율적으로 다루기 위한 Pandas의 핵심 기능을 단계별로 학습하며 정리한 기록입니다.

## 🔢 1. NumPy 학습 목차 및 내용 SUMMARY
| 순서 | 주제 | 파일명 (.ipynb) | 주요 학습 내용 |
| :--- | :--- | :--- | :--- |
| 01 | NumPy 기본 특징 | `ex01_numpy_기본.ipynb` | • import numpy as np 라이브러리 호출<br>• Python List vs NumPy ndarray 메모리 및 속도 비교<br>• 다차원(N차원) 데이터 구조 지원 |
| 02 | 배열 생성 및 속성 | `ex02_배열_생성_속성.ipynb` | • 배열 생성 (np.array, np.zeros, np.full, np.arange)<br>• 난수 생성 (np.random.randint)<br>• 핵심 속성 확인 (shape, size, ndim) |
| 03 | 연산 & 브로드캐스팅 | `ex03_배열_연산.ipynb` | • 원소별 연산 (Element-wise operations)<br>• 형태가 다른 배열 간 자동 확장 연산 (Broadcasting) |
| 04 | 인덱싱 & 슬라이싱 | `ex04_인덱싱_슬라이싱.ipynb` | • 다차원 인덱싱 (`arr[행, 열]`) 및 슬라이싱 (`arr[행범위, 열범위]`)<br>• 조건식 기반 데이터 필터링 (Boolean Indexing) |
| 05 | 데이터 분석 실습 | `ex05_numpy_실습.ipynb` | • BMI 지수 일괄 계산 실습 (단위 변환 및 공식 적용)<br>• 영화 평점 데이터 분석 (np.loadtxt, np.unique, 평점 필터링) |

### 💡 NumPy 주요 개념 정리
1. **NumPy와 ndarray**
   - **ndarray:** 동일한 자료형만 담을 수 있는 고성능 N차원 배열 객체로, 파이썬 리스트에 비해 메모리 효율이 높고 연산 속도가 매우 빠름
2. **배열 생성 및 속성 확인**
   - **배열 생성 함수:** `zeros` (0으로 채움), `full` (특정 값 지정), `arange` (연속 수열), `random.randint` (정수 난수)
   - **핵심 속성:** `shape` (형태 및 크기), `size` (전체 요소 수), `ndim` (차원 수)
3. **원소별 연산 및 브로드캐스팅 (Broadcasting)**
   - **원소별 연산:** 반복문 없이 동일한 위치의 원소끼리 연산 수행
   - **브로드캐스팅:** 형태가 다른 배열끼리 연산 시 자동으로 크기를 확장하여 계산
4. **불리언 인덱싱 (Boolean Indexing)**
   - 조건식을 통해 True / False 마스크를 생성하고, True인 원소만 빠르게 추출
5. **데이터 분석 실습 핵심 함수**
   - `np.loadtxt()` : 텍스트/CSV 포맷의 수치 데이터를 다차원 배열로 로드
   - `np.mean()` / `np.unique()` : 평균 계산 및 중복 없는 고유값 추출

---

## 🐼 2. Pandas 학습 목차 및 내용 SUMMARY
| 순서 | 주제 | 파일명 (.ipynb) | 주요 학습 내용 |
| :--- | :--- | :--- | :--- |
| 01 | Pandas 기본 구조 | `ex01_pandas_기본.ipynb` | • import pandas as pd 라이브러리 호출<br>• 1차원 구조 Series 및 2차원 구조 DataFrame 생성<br>• DataFrame 기본 속성 (head, tail, shape, info, describe) |
| 02 | 데이터 선택 & 필터링 | `ex02_데이터_선택.ipynb` | • 열(Column) 및 행(Row) 선택 (`loc`, `iloc`)<br>• 조건식을 활용한 불리언 인덱싱 및 데이터 추출 |
| 03 | 데이터 정제 & 가공 | `ex03_데이터_정제.ipynb` | • 결측치(NaN) 확인 및 처리 (`dropna`, `fillna`)<br>• 중복 데이터 제거 및 데이터 타입(Type) 변환 |
| 04 | 그룹화 & 집계 연산 | `ex04_그룹화_연산.ipynb` | • `groupby()`를 이용한 데이터 그룹화<br>• 집계 함수 적용 (`mean`, `sum`, `count`, `agg`) |
| 05 | 파일 입출력 & 실습 | `ex05_pandas_실습.ipynb` | • CSV, Excel 파일 읽기 및 쓰기 (`read_csv`, `to_csv`)<br>• 실제 공공 데이터(또는 실습용 데이터셋) 전처리 및 분석 종합 실습 |

### 💡 Pandas 주요 개념 정리
1. **Series와 DataFrame**
   - **Series:** 1차원 배열 형태의 데이터 구조로, 값(Value)과 인덱스(Index)로 구성
   - **DataFrame:** 2차원 행렬(표) 형태의 데이터 구조로, 여러 개의 Series가 모여서 구성된 데이터 분석의 핵심 객체
2. **데이터 선택 및 인덱싱 (`loc` vs `iloc`)**
   - **`loc`:** 라벨(Label) 이름을 기준으로 행과 열에 접근
   - **`iloc`:** 정수 인덱스(Integer Position)를 기준으로 행과 열에 접근
3. **데이터 정제 (Data Cleaning)**
   - **결측치 처리:** `isnull()`로 결측치 확인 후 `dropna()`로 제거하거나 `fillna()`로 대체
   - **데이터 변환:** `astype()`을 통한 데이터 타입 변경 및 `map()`, `apply()`를 활용한 커스텀 함수 적용
4. **그룹 분석 (Groupby)**
   - 데이터를 특정 기준으로 묶어 통계치나 요약 정보를 산출하는 과정 (`groupby()` + 집계 함수)
5. **입출력 (I/O)**
   - `pd.read_csv()`와 `df.to_csv()`를 활용하여 외부 파일과 데이터 교환