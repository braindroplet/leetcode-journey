# leetcode-journey

Solving LeetCode one problem at a time. Consistency over perfection.

---

## 🌟 Week 1: 복잡도 분석 & 배열·문자열

| Day    | 문제                                                      | 링크                                                                 | 난이도 | 학습 포인트                                                       | 완료 |
|:------:|:----------------------------------------------------------|:---------------------------------------------------------------------|:------:|:------------------------------------------------------------------|:-----|
| Day 1  | Running Sum of 1d Array                                   | https://leetcode.com/problems/running-sum-of-1d-array/               | Easy   | Prefix Sum 패턴<br>O(n) 시간·O(1) 공간                            | ☐    |
| Day 2  | Two Sum                                                   | https://leetcode.com/problems/two-sum/                               | Easy   | HashMap 보완 검색 패턴<br>O(n) 시간·O(n) 공간                      | ☐    |
| Day 3  | Reverse String                                            | https://leetcode.com/problems/reverse-string/                        | Easy   | Two‑pointer in‑place 뒤집기<br>char 배열 vs StringBuilder          | ☐    |
| Day 4  | Valid Palindrome                                          | https://leetcode.com/problems/valid-palindrome/                      | Easy   | 문자열 전처리 + 투-포인터 유효성 검사                             | ☐    |
| Day 5  | Container With Most Water                                 | https://leetcode.com/problems/container-with-most-water/             | Medium | 양끝 투-포인터로 최적 해 탐색                                     | ☐    |
| Day 6  | Longest Substring Without Repeating Characters            | https://leetcode.com/problems/longest-substring-without-repeating-characters/ | Medium | 슬라이딩 윈도우 + Map으로 인덱스 관리                             | ☐    |
| Day 7  | **복습 & 리팩토링**                                        | —                                                                    | —      | 각 풀이 복잡도 문서화<br>코드 클린업 (불필요 객체 제거)           | ☐    |

---

## 🌟 Week 2: 재귀(Recursion) & 이분 탐색

| Day       | 문제                             | 링크                                                                    | 난이도 | 학습 포인트                                                        | 완료 |
|:---------:|:--------------------------------|:------------------------------------------------------------------------|:------:|:-------------------------------------------------------------------|:-----|
| Day 8     | Fibonacci Number                | https://leetcode.com/problems/fibonacci-number/                         | Easy   | 단순 재귀 vs 탑다운 메모이제이션 비교                             | ☐    |
| Day 9     | Merge Two Sorted Lists          | https://leetcode.com/problems/merge-two-sorted-lists/                   | Easy   | 연결 리스트 병합(분할 정복)                                      | ☐    |
| Day 10    | Binary Search                   | https://leetcode.com/problems/binary-search/                            | Easy   | 반복 vs 재귀 이진 탐색 구현<br>O(log n) 이해                      | ☐    |
| Day 11    | Search in Rotated Sorted Array  | https://leetcode.com/problems/search-in-rotated-sorted-array/           | Medium | Pivot 처리한 변형 이분 탐색                                       | ☐    |
| Day 12    | **복습 & 예제 변형**             | —                                                                      | —      | 메모이제이션 vs 단순 재귀 성능 측정<br>경계 조건 테스트 케이스 추가 | ☐    |
| Day 13–14 | **주말 리뷰**                    | —                                                                      | —      | Week 1–2 핵심 노트 정리<br>GitHub 커밋 & README 업데이트           | ☐    |

---

## 🌟 Week 3: 자료구조 & 그래프 탐색

| Day    | 문제                           | 링크                                                       | 난이도 | 학습 포인트                                           | 완료 |
|:------:|:------------------------------|:-----------------------------------------------------------|:------:|:------------------------------------------------------|:-----|
| Day 15 | Valid Parentheses             | https://leetcode.com/problems/valid-parentheses/           | Easy   | Stack으로 괄호 매칭                                   | ☐    |
| Day 16 | Add Two Numbers               | https://leetcode.com/problems/add-two-numbers/             | Medium | 연결 리스트 덧셈 + 자리올림 처리                      | ☐    |
| Day 17 | Longest Consecutive Sequence  | https://leetcode.com/problems/longest-consecutive-sequence/ | Medium | HashSet으로 연속 수열 탐색                            | ☐    |
| Day 18 | Number of Islands             | https://leetcode.com/problems/number-of-islands/           | Medium | DFS/BFS로 그리드 탐색 + 방문 처리                    | ☐    |
| Day 19 | Course Schedule               | https://leetcode.com/problems/course-schedule/             | Medium | 위상 정렬/Union‑Find로 사이클 검출                    | ☐    |
| Day 20 | **복습 & 그래프 구현**         | —                                                          | —      | 인접 리스트 vs 행렬 구현 비교<br>코드에 주석으로 방문 순서 표시 | ☐    |
| Day 21 | **주말 리뷰**                  | —                                                          | —      | Week 3 전체 개념 맵 작성<br>혼자 설명해 보기            | ☐    |

---

## 🌟 Week 4: 동적 계획법(DP) & 그리디

| Day    | 문제                                | 링크                                                         | 난이도 | 학습 포인트                                                   | 완료 |
|:------:|:-----------------------------------|:-------------------------------------------------------------|:------:|:--------------------------------------------------------------|:-----|
| Day 22 | Climbing Stairs                     | https://leetcode.com/problems/climbing-stairs/                | Easy   | 점화식 설계<br>탑다운 vs 바텀업 비교                          | ☐    |
| Day 23 | House Robber                        | https://leetcode.com/problems/house-robber/                   | Medium | 상태 전이(state machine) DP 모델링                            | ☐    |
| Day 24 | Longest Increasing Subsequence      | https://leetcode.com/problems/longest-increasing-subsequence/ | Medium | O(n²) DP vs O(n log n) 이분 탐색 최적화                       | ☐    |
| Day 25 | Assign Cookies                      | https://leetcode.com/problems/assign-cookies/                 | Easy   | 그리디 매칭 설계<br>정렬 + 투-포인터                           | ☐    |
| Day 26 | Top K Frequent Elements             | https://leetcode.com/problems/top-k-frequent-elements/        | Medium | Heap(PriorityQueue) 기반 빈도 정렬                            | ☐    |
| Day 27 | **복습 & 모의 인터뷰**               | —                                                            | —      | 30분 타임박스, Medium 2문제 풀기                              | ☐    |
| Day 28 | **최종 리뷰 & 계획 수립**            | —                                                            | —      | GitHub 최종 커밋<br>취약 단원 추가 보강 계획                  | ☐    |
