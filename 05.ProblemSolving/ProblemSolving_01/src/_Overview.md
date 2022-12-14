Wrap-up
===

문제 설명
---

<h3> 코딩테스트 개요 </h3>
문제 해석 -> 문제 풀이 -> 프로그램 채점 (w/ Test Case)

```text
* 문제 해석
  * 주어진 문제를 잘 이해해서 무엇을 푸는 문제인지 정확히 파악
  * 입출력 범위와 타입 및 조건사항 체크
  
* 문제 풀이
  * 풀이 전략 구상
  * 알고리즘 선택
  
* 프로그램 채점
  * Pass -> 해당 Test case 통과
  * 컴파일 에러 (CE) -> 구문 오류
  * Fail -> 풀이 방법 틀림
  * TLE (Time Limit Error) -> 시간복잡도 개선 필요
  * MLE (Memory Limit Error) -> 공간복잡도 개선 필요
```

<br/>
<br/>


<h3> 입출력 값 범위에 대한 자료형 확인 </h3>

| 자료형    | 크기(Byte) | 범위                                                     |
|--------|----------|--------------------------------------------------------|
| byte   | 1        | -128 ~ 127                                             |
| short  | 2        | -32,768 ~ 32,767                                       |
| int    | 4        | -2,147,483,648 ~ 2,147,483,647                         |
| long   | 8        | -9,223,372,036,854,775,808 ~ 9,223,372,036,854,775,807 |
| float  | 4        | ±1.4E-45 ~ 3.4E38                                      |
| double | 8        | ±4.9E-324 ~ 1.8E308                                    |

<br/>
<br/>


<h3> 입력 값의 범위와 시간 복잡도 </h3>

```text
* 문제 풀이 제한 시간 1초인 경우,
  - 입력 값 범위가 1,000 이내 -> 시간 복잡도 O(N³) 이하로 실행 가능
  - 입력 값 범위가 10,000 이내 -> 시간 복잡도 O(N²) 이하로 실행 가능
  - 입력 값 범위가 100,000 이내 -> 시간 복잡도 O(NlogN) 이하로 실행 가능
  - 입력 값 범위가 10,000,000 이내 -> 시간 복잡도 O(N) 이하로 실행 가능
```

<br/>
<br/>


<h3> 메모리 제약 조건 체크 </h3>

```java
int a;                              // 4 byte
int[] a = new int[1000];            // 4KB
int[] a = new int[1_000_000];       // 4MB
int[][]a = new int[10_000][10_000]; // 400MB

```

