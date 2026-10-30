---
name: plan-doc
description: Use at the start of a task, before writing any code, to turn the task statement into PLAN.md with a requirements checklist, decisions, schedule, verification method, and open questions. Also use when the plan must be revised after a requirement changes.
---

# plan-doc

과제 설명을 읽고 프로젝트 루트에 PLAN.md를 만든다. 이미 있으면 바뀐 부분만 고친다.

## 입력
- 과제 설명 (사용자가 붙여넣거나 파일로 제공)
- 남은 시간 (사용자에게 묻거나 사용자가 알려준 값)

## PLAN.md 구조
```
# PLAN
## 목표
한두 문장. 무엇을 누구를 위해 만드는가.

## 요구사항 체크리스트
- [ ] R1 ... (과제 문장에서 그대로 가져온 근거를 괄호로)
- [ ] R2 ...

## 판단과 근거
- 기술 선택: 무엇을 왜 (다른 선택지보다 나은 이유 한 줄)
- 범위: 이번에 하지 않을 것과 이유

## 작업 순서 (30~40분 단위)
1. ... (끝났다고 판단하는 기준)
2. ...

## 시간 배분
- 마지막 30분: 검증과 문서 정리
- 마지막 10분: 제출

## 검증 방법
- 요구사항별로 어떻게 확인할지 (명령어, 화면, 입력 예시)

## 모르는 것 / 위험
- 실무자 에이전트에게 물어볼 질문
- 시간이 모자랄 때 먼저 버릴 것
```

## 규칙
- 요구사항은 과제 문장에 근거가 있는 것만 적는다. 추측한 요구사항은 "모르는 것"으로 보낸다.
- 작업 순서는 핵심 기능이 먼저, 꾸미기는 마지막.
- 작성 후 사용자에게 요약 5줄과 질문 목록만 보여준다.
