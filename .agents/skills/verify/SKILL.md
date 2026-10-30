---
name: verify
description: Use when a feature or work step is finished and must be checked before calling it done. Runs tests or build, checks a running server, guides a browser check, and updates the requirements checklist.
---

# verify

방금 끝낸 작업이 실제로 동작하는지 확인한다. 확인 결과는 `$decision-log`로 DECISIONS.md에 남긴다.

## 순서
1. 테스트나 빌드가 있으면 실행한다. 실패하면 여기서 멈추고 실패 출력을 보여준다.
2. 웹 서버가 있으면:
   - 서버가 `0.0.0.0`에 바인딩됐는지 확인한다.
   - `curl -s -o /dev/null -w '%{http_code}' http://0.0.0.0:<포트>/<경로>`로 응답 코드를 확인한다.
   - API면 대표 요청 하나를 보내고 응답 본문 일부를 확인한다.
3. 화면이 있으면 사용자에게 IDE의 Browser 탭에서 확인할 것을 한 줄씩 알려준다 (어디를 누르고 무엇이 보여야 하는지).
4. PLAN.md 요구사항 체크리스트에서 확인된 항목만 체크한다.

## 보고 형식
- 통과: 무엇을 어떻게 확인했나 (명령어와 결과)
- 실패/미확인: 무엇이 안 됐고 다음에 할 일
- 체크한 요구사항 번호

## 규칙
- 실행하지 않은 확인을 통과로 적지 않는다.
- 테스트를 지우거나 건너뛰어서 통과시키지 않는다.
