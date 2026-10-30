---
name: decision-log
description: Use after finishing each work step, after any technical choice, and after each verification, to append one entry to DECISIONS.md recording what was done, why, how it was checked, and what limits remain.
---

# decision-log

프로젝트 루트의 DECISIONS.md 끝에 항목 하나를 추가한다. 파일이 없으면 만든다. 기존 항목은 고치지 않는다.

## 항목 형식
```
## D<번호>. <한 줄 제목> (<시각 HH:MM>)
- 한 것: 무엇을 바꿨나 (파일, 기능)
- 이유: 왜 이렇게 했나. 고려한 다른 방법과 그걸 고르지 않은 이유
- 확인: 실행한 명령어나 확인한 화면, 그리고 결과 (통과/실패, 숫자)
- 한계: 아직 안 되는 것, 가정한 것, 시간이 있으면 할 것
```

## 규칙
- 짧게. 항목 하나에 6줄 이내.
- "확인"에는 실제로 실행한 것만 쓴다. 실행하지 않았으면 "미확인"이라고 쓴다.
- 요구사항 체크리스트(PLAN.md)의 어떤 항목과 관련 있는지 R번호를 제목에 붙인다.
- 사용자가 나중에 이 파일만 읽고 "왜 이렇게 했는지" 설명할 수 있어야 한다.
