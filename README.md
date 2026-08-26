# 🐍 Python 학습 일지 (Study Log)
파이썬 기초 문법 및 활용법을 단계별로 학습하며 정리한 기록입니다.

## 📅 학습 목차 및 내용 SUMMARY
| 순서 | 주제 | 파일명 (.ipynb) | 주요 학습 내용 |
| :---: | :--- | :--- | :--- |
| 01 | 변수 & 문자열 | ex01_변수, 문자열.ipynb | • 변수 선언 및 메모리 개념<br>• 문자열 인덱싱 & 슬라이싱<br>• 문자열 포맷팅 (f-string) 및 주요 메서드 |
| 02 | 연산자 | ex02_연산자.ipynb | • 산술, 대입, 비교, 논리 연산자<br>• 연산자 우선순위 및 활용 |
| 03 | 조건문 | ex03_조건문.ipynb | • if, elif, else 제어문 구조<br>• 조건 판단식 작성 및 중첩 조건문 |
| 04 | 리스트 & 튜플 | ex04_리스트, 튜플.ipynb | • 리스트/튜플 생성, 수정, 삭제<br>• 요솟값 추가, 정렬 등의 메서드<br>• Mutability(가변성) vs Immutability(불변성) |
| 05 | 반복문 | ex05_반복문.ipynb | • for 문과 while 문 활용<br>• range() 함수 및 리스트 내포 (List Comprehension)<br>• break, continue 흐름 제어 |
| 06 | 딕셔너리 | ex06_딕셔너리.ipynb | • Key-Value 구조의 데이터 관리<br>• keys(), values(), items() 활용 |
| 07 | 함수 | ex07_함수.ipynb | • 사용자 정의 함수 (def) 및 반환값 (return)<br>• 매개변수 (\*args, \*\*kwargs) 및 Lambda 표현식 |

## 💡 주요 개념 정리
1. **변수와 문자열**
* • **변수**: 데이터를 저장하는 메모리 공간의 이름
* • **문자열 슬라이싱**: string[start:end:step] 구문을 통한 부분 문자열 추출

2. **연산자**
* • **산술 연산자**: +, -, \*, /, // (몫), % (나머지), \*\* (거듭제곱)
* • **논리 연산자**: and, or, not

3. **조건문**
* • **조건 제어**: 조건에 따라 프로그램 실행 흐름을 제어 (if - elif - else)

4. **리스트 vs 튜플**
* • **리스트 ([])**: 요소를 자유롭게 추가/수정/삭제 가능 (Mutable)
* • **튜플 (())**: 한번 생성되면 요소를 변경할 수 없음 (Immutable)

5. **반복문**
* • **for 문**: 정해진 횟수나 순회 가능한(Iterable) 객체를 순차적으로 반복
* • **while 문**: 조건식이 True인 동안 지속적으로 반복 실행

6. **딕셔너리**
* • **딕셔너리 ({key: value})**: Key와 Value의 쌍으로 구성된 데이터 구조며, Key를 통해 빠르게 값에 접근 가능 (Key 중복 불가)

7. **함수**
* • **사용자 정의 함수 (def)**: 코드의 재사용성을 높이기 위해 특정 기능을 수행하는 코드 블록을 정의
* • **매개변수 (\*args, \*\*kwargs)**: 가변 인수를 받아 다양한 개수의 데이터를 처리 가능
* • **람다 표현식 (lambda)**: 이름 없는 익명 함수를 간결하게 한 줄로 작성할 때 사용

### 2. 주요 데이터 구조 비교 (Data Structures)
* • 🟢 **리스트 (list)**: [1, 2, 3] — 순서 O, 중복 O, 수정 가능 (Mutable)
* • 🔴 **튜플 (tuple)**: (1, 2, 3) — 순서 O, 중복 O, 수정 불가 (Immutable)
* • 🟡 **딕셔너리 (dict)**: {"key": "value"} — Key-Value 쌍, Key 중복 불가

---

# 🔢 파이썬 라이브러리 학습 일지 (NumPy, Pandas & Matplotlib)
고성능 다차원 배열 연산 및 수치 데이터 분석 라이브러리인 NumPy, 표 형태의 데이터를 직관적이고 효율적으로 다루기 위한 Pandas, 그리고 데이터 시각화를 위한 Matplotlib의 핵심 기능을 단계별로 학습하며 정리한 기록입니다.

## 📅 1. NumPy 학습 목차 및 내용 SUMMARY
| 순서 | 주제 | 파일명 (.ipynb) | 주요 학습 내용 |
| :---: | :--- | :--- | :--- |
| 01 | NumPy 기본 특징 | ex01_numpy_기본.ipynb | • import numpy as np 라이브러리 호출<br>• Python List vs NumPy ndarray 메모리 및 속도 비교<br>• 다차원(N차원) 데이터 구조 지원 |
| 02 | 배열 생성 및 속성 | ex02_배열_생성_속성.ipynb | • 배열 생성 (np.array, np.zeros, np.full, np.arange)<br>• 난수 생성 (np.random.randint)<br>• 핵심 속성 확인 (shape, size, ndim) |
| 03 | 연산 & 브로드캐스팅 | ex03_배열_연산.ipynb | • 원소별 연산 (Element-wise operations)<br>• 형태가 다른 배열 간 자동 확장 연산 (Broadcasting) |
| 04 | 인덱싱 & 슬라이싱 | ex04_인덱싱_슬라이싱.ipynb | • 다차원 인덱싱 (arr[행, 열]) 및 슬라이싱 (arr[행범위, 열범위])<br>• 조건식 기반 데이터 필터링 (Boolean Indexing) |
| 05 | 데이터 분석 실습 | ex05_numpy_실습.ipynb | • BMI 지수 일괄 계산 실습 (단위 변환 및 공식 적용)<br>• 영화 평점 데이터 분석 (np.loadtxt, np.unique, 평점 필터링) |

## 💡 NumPy 주요 개념 정리
1. **NumPy와 ndarray**
* • **ndarray**: 동일한 자료형만 담을 수 있는 고성능 N차원 배열 객체로, 파이썬 리스트에 비해 메모리 효율이 높고 연산 속도가 매우 빠름

2. **배열 생성 및 속성 확인**
* • **배열 생성 함수**: zeros (0으로 채움), full (특정 값 지정), arange (연속 수열), random.randint (정수 난수)
* • **핵심 속성**: shape (형태 및 크기), size (전체 요소 수), ndim (차원 수)

3. **원소별 연산 및 브로드캐스팅 (Broadcasting)**
* • **원소별 연산**: 반복문 없이 동일한 위치의 원소끼리 연산 수행
* • **브로드캐스팅**: 형태가 다른 배열끼리 연산 시 자동으로 크기를 확장하여 계산

4. **불리언 인덱싱 (Boolean Indexing)**
* • **조건식 필터링**: 조건식을 통해 True/False 마스크를 생성하고, True인 원소만 빠르게 추출

5. **데이터 분석 실습 핵심 함수**
* • **np.loadtxt()**: 텍스트/CSV 포맷의 수치 데이터를 다차원 배열로 로드
* • **np.mean() / np.unique()**: 평균 계산 및 중복 없는 고유값 추출

---

## 🐼 2. Pandas 학습 목차 및 내용 SUMMARY
| 순서 | 주제 | 파일명 (.ipynb) | 주요 학습 내용 |
| :---: | :--- | :--- | :--- |
| 01 | Pandas 기본 구조 | ex01_pandas_기본.ipynb | • import pandas as pd 라이브러리 호출<br>• 1차원 구조 Series 및 2차원 구조 DataFrame 생성<br>• DataFrame 기본 속성 (head, tail, shape, info, describe) |
| 02 | 데이터 선택 & 필터링 | ex02_데이터_선택.ipynb | • 열(Column) 및 행(Row) 선택 (loc, iloc)<br>• 조건식을 활용한 불리언 인덱싱 및 데이터 추출 |
| 03 | 데이터 정제 & 가공 | ex03_데이터_정제.ipynb | • 결측치(NaN) 확인 및 처리 (dropna, fillna)<br>• 중복 데이터 제거 및 데이터 타입(Type) 변환 |
| 04 | 그룹화 & 집계 연산 | ex04_그룹화_연산.ipynb | • groupby() 를 이용한 데이터 그룹화<br>• 집계 함수 적용 (mean, sum, count, agg) |
| 05 | 파일 입출력 & 실습 | ex05_pandas_실습.ipynb | • CSV, Excel 파일 읽기 및 쓰기 (read_csv, to_csv)<br>• 실제 공공 데이터(또는 실습용 데이터셋) 전처리 및 분석 종합 실습 |

## 💡 Pandas 주요 개념 정리
1. **Series와 DataFrame**
* • **Series**: 1차원 배열 형태의 데이터 구조로, 값(Value)과 인덱스(Index)로 구성
* • **DataFrame**: 2차원 행렬(표) 형태의 데이터 구조로, 여러 개의 Series가 모여서 구성된 데이터 분석의 핵심 객체

2. **데이터 선택 및 인덱싱 (loc vs iloc)**
* • **loc**: 라벨(Label) 이름을 기준으로 행과 열에 접근
* • **iloc**: 정수 인덱스(Integer Position)를 기준으로 행과 열에 접근

3. **데이터 정제 (Data Cleaning)**
* • **결측치 처리**: isnull()로 결측치 확인 후 dropna()로 제거하거나 fillna()로 대체
* • **데이터 변환**: astype()을 통한 데이터 타입 변경 및 map(), apply()를 활용한 커스텀 함수 적용

4. **그룹 분석 (Groupby)**
* • **그룹 연산**: 데이터를 특정 기준으로 묶어 통계치나 요약 정보를 산출하는 과정 (groupby() + 집계 함수)

5. **입출력 (I/O)**
* • **파일 교환**: pd.read_csv()와 df.to_csv()를 활용하여 외부 파일과 데이터 교환

---

## 📊 3. Matplotlib 학습 목차 및 내용 SUMMARY
| 순서 | 주제 | 파일명 (.ipynb) | 주요 학습 내용 |
| :---: | :--- | :--- | :--- |
| 01 | Matplotlib 기본 구조 | ex01_matplotlib_기본.ipynb | • import matplotlib.pyplot as plt 라이브러리 호출<br>• 기본 선 그래프(Line Plot) 그리기 및 plt.show()<br>• 타이틀, 축 라벨(xlabel, ylabel), 범례(legend) 설정 |
| 02 | 다양한 차트 시각화 | ex02_차트_종류.ipynb | • 산점도(scatter), 막대 그래프(bar), 히스토그램(hist) 작성<br>• 데이터 특성에 맞는 적절한 시각화 기법 선택 |
| 03 | 스타일 및 서브플롯 | ex03_스타일_서브플롯.ipynb | • 선 스타일, 마커, 색상(color, linestyle, marker) 커스텀<br>• plt.subplots() 를 활용한 다중 그래프(Subplot) 배치 및 관리 |

## 💡 Matplotlib 주요 개념 정리
1. **기본 시각화와 요소 설정**
* • **선 그래프 (plt.plot())**: 데이터의 추세와 흐름을 시각적으로 파악하기 위한 기본 그래프
* • **축 및 레이블 설정**: plt.title(), plt.xlabel(), plt.ylabel()을 통해 그래프의 가독성 향상

2. **다양한 차트 활용**
* • **막대 그래프 (plt.bar())**: 범주별 비교 데이터 시각화
* • **산점도 (plt.scatter())**: 두 변수 간의 상관관계 및 분포 확인

3. **다중 그래프 표현 (Subplot)**
* • **다중 배치**: plt.subplots()를 활용하여 하나의 창에 여러 개의 그래프를 분할하여 배치하고 비교 분석 수행

---

# 💻 HTML/CSS 학습 일지 (Study Log)
웹 페이지의 뼈대를 구성하는 구조 설계 언어인 HTML과 디자인 및 스타일을 입히는 CSS의 핵심 기능을 단계별로 학습하며 정리한 기록입니다.

## 📅 1. HTML 학습 목차 및 내용 SUMMARY
| 순서 | 주제 | 파일명 (.html) | 주요 학습 내용 |
| :---: | :--- | :--- | :--- |
| 01 | HTML 기본 구조 | ex01_basic.html | • HTML 문서 기본 틀 (!DOCTYPE html, html, head, body)<br>• 기본 태그 (제목 h1~h6, 단락 p, 줄바꿈 br, 수평선 hr) |
| 02 | 텍스트 및 링크 태그 | ex02_text_link.html | • 텍스트 강조 (strong, em)<br>• 하이퍼링크 (a) 및 이미지 삽입 (img) |
| 03 | 목록 및 테이블 태그 | ex03_list_table.html | • 순서 없는 목록 (ul), 순서 있는 목록 (ol), 항목 (li)<br>• 표 생성 태그 (table, tr, th, td) 및 셀 병합 |
| 04 | 입력 폼 및 시맨틱 태그 | ex04_form_semantic.html | • 사용자 입력 폼 (form, input, textarea, button)<br>• 시맨틱 웹 태그 (header, nav, section, article, footer) |

## 💡 HTML 주요 개념 정리
1. **HTML 기본 구조**
* • **태그(Tag) 구조**: 콘텐츠를 감싸서 웹 브라우저가 구조를 이해할 수 있도록 마크업하는 방식 (<태그명>내용</태그명>)
* • **시맨틱 웹(Semantic Web)**: 의미론적 태그를 사용하여 웹 페이지의 구조와 목적을 명확히 전달하는 설계 방식

2. **핵심 태그 활용**
* • **링크와 이미지**: a 태그의 href 속성으로 페이지 이동, img 태그의 src와 alt 속성으로 이미지 및 대체 텍스트 지정
* • **폼(Form)**: 사용자의 입력을 받아 서버로 데이터를 전송하는 인터페이스 구성

---

## 📅 2. CSS 학습 목차 및 내용 SUMMARY
| 순서 | 주제 | 파일명 (.css / .html) | 주요 학습 내용 |
| :---: | :--- | :--- | :--- |
| 01 | CSS 기본 및 선택자 | ex01_selector.html | • CSS 적용 방식 (Inline, Internal, External)<br>• 기본 선택자 (전체, 태그, 아이디 #, 클래스 .) |
| 02 | 박스 모델 (Box Model) | ex02_boxmodel.html | • 요소의 4가지 영역 (Content, Padding, Border, Margin)<br>• box-sizing 속성 (border-box 활용법) |
| 03 | 레이아웃 및 배치 | ex03_layout.html | • 화면 배치 속성 (display: block, inline, none)<br>• Flexbox 모델 (display: flex, justify-content, align-items) |
| 04 | 디자인 및 반응형 | ex04_responsive.html | • 폰트, 색상, 배경 설정<br>• 미디어 쿼리(@media)를 활용한 반응형 웹 디자인 기초 |

## 💡 CSS 주요 개념 정리
1. **선택자 (Selectors)**
* • **클래스(.) vs 아이디(#)**: 클래스는 중복 사용 가능하며 여러 개 지정 가능, 아이디는 페이지 내 고유한 단 하나의 요소에만 지정

2. **박스 모델 (Box Model)**
* • **박스 구성**: 모든 HTML 요소를 사각형 박스로 간주하며, 안쪽 여백(padding), 테두리(border), 바깥쪽 여백(margin)으로 구성

3. **Flexbox 레이아웃**
* • **정렬 시스템**: 행과 열 방향으로 요소를 유연하게 정렬하고 간격을 제어할 수 있는 현대적인 레이아웃 시스템 (justify-content로 수평 정렬, align-items로 수직 정렬)

---

# 💻 JavaScript 학습 일지 (Study Log)
웹 페이지를 동적으로 제어하고 사용자 인터랙션을 구현하는 프로그래밍 언어인 자바스크립트(JavaScript)의 핵심 기능을 단계별로 학습하며 정리한 기록입니다.

## 📅 학습 목차 및 내용 SUMMARY
| 순서 | 주제 | 파일명 (.js / .html) | 주요 학습 내용 |
| :---: | :--- | :--- | :--- |
| 01 | 기본 입출력문 | ex01_io.html | • script 태그 활용<br>• 입력 기능 (prompt, confirm) 및 출력 기능 (console.log, alert, document.write)<br>• 템플릿 리터럴(Template Literal) 활용 |
| 02 | 변수 선언 키워드 | ex02_variable.js | • 변수 선언 키워드 비교 (var, let, const)<br>• 변수명 재사용 및 재할당 특성 이해 |
| 03 | 자료형 | ex03_datatype.js | • 원시 자료형 (숫자형, 문자열, 논리형, undefined, null)<br>• 참조 자료형 (배열 Array, 객체 Object)<br>• typeof 연산자를 활용한 자료형 확인 |
| 04 | 형 변환 | ex04_conversion.js | • 자동 형 변환 및 강제 형 변환 (Number, parseInt, parseFloat, String, toString, toFixed) |
| 05 | 연산자 | ex05_operator.js | • 산술, 증감, 비교(== vs ===), 논리, 삼항 연산자 활용 |
| 06 | 조건문 | ex06_condition.js | • 조건 제어문 구조 (if, if ~ else, else if, switch) |
| 07 | 반복문 | ex07_loop.js | • 반복문 활용 (while, for) 및 break 흐름 제어 |
| 08 | 배열 (Array) | ex08_array.js | • 배열 생성, 인덱스 접근 및 주요 메서드 (push, pop, shift, unshift, splice 등)<br>• 배열 고차 함수 (forEach, map, filter, reduce) 활용 |
| 09 | 함수 (Function) | ex09_function.js | • 함수 선언문과 함수 표현식<br>• 화살표 함수(Arrow Function) 문법<br>• 스코프(Scope)와 클로저(Closure) 개념 |
| 10 | 객체 (Object) | ex10_object.js | • 객체 생성 및 속성(Property) / 메서드(Method) 정의<br>• 객체 리터럴과 this 키워드 이해 |
| 11 | 문서 객체 모델 (DOM) | ex11_dom.html | • DOM의 개념과 노드 선택 메서드 (getElementById, querySelector 등)<br>• 요소의 콘텐츠 및 스타일 제어 (innerHTML, textContent, style)<br>• 이벤트 처리 기본 (addEventListener) |
| 12 | 이벤트 (Events) | ex12_event.html | • 마우스, 키보드, 폼 등 다양한 사용자 이벤트 리스너 (addEventListener) 등록<br>• 이벤트 객체(event) 활용 및 이벤트 전파(Bubbling & Capturing) 제어 |
| 13 | 데이터 통신 (Async/Fetch) | ex13_async_fetch.html | • 비동기 통신(Async/Await, Promise) 개념 이해<br>• fetch() API 를 활용한 외부 서버 데이터(JSON) 비동기 요청 및 응답 처리 |

## 💡 주요 개념 정리
1. **기본 입출력문과 템플릿 리터럴**
* • **입출력 함수**: prompt로 문자열 입력을 받고, confirm으로 참·거짓 선택을 받으며, console.log, alert, document.write로 결과 출력 가능
* • **템플릿 리터럴**: 백틱(\`)을 사용하여 변수와 문자열을 간편하게 조합

2. **변수 선언 키워드 (var, let, const)**
* • **var**: 재사용과 재할당이 모두 가능하나 중복 문제로 현재는 지양
* • **let**: 재사용은 불가하지만 값의 재할당이 가능한 일반 변수
* • **const**: 값의 변경이 불가능한 상수

3. **자료형 (Data Types)**
* • **원시 자료형**: 숫자형, 문자열, 논리형, undefined, null
* • **참조 자료형**: 배열(Array), 객체(Object)

4. **형 변환 (Type Conversion)**
* • **강제 형 변환**: Number(), parseInt() 등으로 숫자형 변환, String(), toFixed() 등으로 문자열 및 소수점 제어

5. **연산자 (Operators)**
* • **비교 연산자**: 데이터 값과 자료형을 모두 엄격하게 비교하는 일치 연산자(===) 사용 권장

6. **조건문과 반복문 (Control Statements & Loops)**
* • **조건문**: 상황에 따라 흐름을 제어하는 if, else if, switch 문 활용
* • **반복문**: 횟수가 정해진 반복은 for 문, 특정 조건 하의 반복은 while 문 활용

7. **배열 (Array)**
* • **배열 메서드 및 고차 함수**: push(), pop() 등으로 요소를 다루고, map(), filter() 등으로 데이터를 효율적으로 가공

8. **함수 (Function)**
* • **화살표 함수**: 기존 함수 선언 방식을 간결하게 표현하며, 스코프와 클로저를 통해 변수의 유효 범위와 상태 관리

9. **객체 (Object)**
* • **객체와 this**: 키-값 쌍으로 데이터를 묶고, 메서드 내부에서 this를 통해 객체 자신의 속성에 접근

10. **DOM (Document Object Model)**
* • **요소 선택 및 조작**: querySelector 등으로 요소를 선택하고, 동적 웹 페이지 구현

11. **이벤트 (Events)**
* • **addEventListener()**: 웹 브라우저에서 발생하는 사용자의 행동(클릭, 입력 등)이나 상태 변화를 감지하여 이벤트 핸들러 실행
* • **이벤트 객체**: 발생한 이벤트의 상세 정보를 담고 있으며, event.preventDefault() 등으로 기본 동작 제어

12. **데이터 통신 (Async/Fetch)**
* • **fetch() API**: 프론트엔드에서 서버와 HTTP 요청을 주고받기 위한 현대적인 자바스크립트 내장 함수
* • **async / await**: 콜백 지옥을 해결하고 동기 코드처럼 직관적으로 서버로부터 데이터를 받아와(JSON 파싱) 웹 화면을 비동기 처리

# 🐍 Flask 웹 서버 학습 일지 (Study Log)

파이썬 기반의 Flask 웹 서버를 구축하고, 클라이언트와 서버 간의 데이터 통신(GET/POST) 원리를 학습하며 정리한 기록입니다.

---

## 📅 학습 목차 및 내용 SUMMARY

| 순서 | 주제 | 파일명 (.py / .html) | 주요 학습 내용 |
| :---: | :--- | :--- | :--- |
| **01** | **Flask 서버 기초** | `ex01_flask_basic.py`<br>`templates/` / `static/` | • Flask 서버 설계도 호출 및 기본 구조 작성<br>• 정적 파일 및 템플릿 파일 관리 폴더 세팅 |
| **02** | **라우팅 및 HTML 응답** | `ex02_route_html.py`<br>`index.html` / `sub.html` | • 여러 개의 라우트(`/`, `/sub`) 경로 설정<br>• `render_template`을 활용한 HTML 문서 응답 |
| **03** | **GET 방식 데이터 통신** | `ex03_get_login.py`<br>`login.html` | • URL에 데이터를 탑재하는 GET 방식 이해<br>• `request.args.get()`을 통한 데이터 추출 |
| **04** | **POST 방식 데이터 통신** | `ex04_post_login.py`<br>`login.html` | • HTTP Body에 데이터를 숨겨 전송하는 POST 방식 이해<br>• `request.form.get()`을 통한 데이터 추출 |

---

## 💡 주요 개념 정리

1. **Flask 서버 기본 구조**
   - **서버 설계도 호출** : `app = Flask(__name__)`을 통해 현재 파일을 기준으로 서버 인스턴스를 생성
   - **라우트(Route) 설정** : `@app.route()`를 사용하여 사용자가 요청한 경로에 따라 적절한 함수와 응답을 매핑
   - **서버 실행** : `app.run(host='localhost', port=5000)`을 통해 로컬 환경에서 서버를 구동 (포트 5000번 관습적 사용)

2. **폴더 구조 및 파일 관리**
   - **`templates/` 폴더** : `render_template()` 함수가 자동으로 탐색하여 HTML 페이지를 렌더링하는 디렉토리
   - **`static/` 폴더** : 이미지, CSS, JS 등의 정적(Static) 파일들을 관리하는 디렉토리

3. **데이터 통신 방식 (GET vs POST)**
   - **GET 방식** : 데이터를 URL 뒤에 쿼리 스트링(`?id=smhrd&pw=1234`) 형태로 탑재하여 전송하며, `request.args.get('key')`로 추출
   - **POST 방식** : 데이터를 HTTP 메시지 Body에 숨겨서 전송하므로 보안과 대용량 전송에 적합하며, `request.form.get('key')`로 추출