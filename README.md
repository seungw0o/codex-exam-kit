# codex-exam-kit

Codex로 시간 제한 있는 개발 과제를 할 때 쓰는 작업 규칙(AGENTS.md)과 작업 방식 스킬 4개. 코드 템플릿이나 과제 풀이는 들어 있지 않다.

## 설치
```bash
git clone https://github.com/seungw0o/codex-exam-kit ~/kit \
  && mkdir -p ~/.agents/skills ~/.codex \
  && cp -r ~/kit/.agents/skills/* ~/.agents/skills/ \
  && cp ~/kit/AGENTS.md ~/.codex/AGENTS.md
```
Codex를 다시 켜고 `/skills`로 목록을 확인한다.

## 구성
- `AGENTS.md`: 모든 작업에 적용되는 규칙 (계획 → 작은 단위 → 검증 → 기록 → 제출)
- `.agents/skills/plan-doc`: 과제 설명으로 PLAN.md 작성
- `.agents/skills/decision-log`: 단계마다 DECISIONS.md에 판단·근거·확인·한계 기록
- `.agents/skills/verify`: 테스트, 서버 응답, 화면 확인 순서
- `.agents/skills/submit`: 마감 전 제출 체크
