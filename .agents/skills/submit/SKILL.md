---
name: submit
description: Use about 15 minutes before the deadline to stop new work and prepare submission. Compares PLAN.md against what was done, checks that submission documents include decisions, reasoning, verification results, and remaining limits, and lists final steps.
---

# submit

새 기능 작업을 멈추고 제출을 준비한다.

## 순서
1. PLAN.md 요구사항 체크리스트를 보고 완료 / 부분 완료 / 미완료로 나눈다.
2. 제출 문서(과제가 요구하는 문서, 없으면 README.md)에 다음 네 가지가 있는지 확인하고 없으면 DECISIONS.md를 바탕으로 채운다:
   - 판단: 주요 기술 선택과 범위 결정
   - 근거: 각 판단의 이유
   - 검증 결과: 실제로 확인한 것과 결과
   - 남은 한계: 미완료 요구사항, 알려진 문제, 가정
3. 서버가 필요한 과제면 서버가 `0.0.0.0`에서 떠 있는지 마지막으로 확인한다.
4. 사용자에게 마지막 할 일을 짧게 알려준다:
   - 제출 버튼 누르기
   - 제출 ID 확인
   - 후속 문항 전에 DECISIONS.md 한 번 읽기

## 규칙
- 이 단계에서 큰 코드 변경을 하지 않는다. 깨진 것을 고치는 최소 변경만.
- 미완료를 완료처럼 쓰지 않는다. 한계는 솔직하게 쓴다.
