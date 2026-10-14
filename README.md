# blog-dock-docs

블로그독(티스토리형 블로그)의 **문서** 저장소. 코드는 [blog-dock](https://github.com/blog-parkseo/blog-dock)에 있다.
[GitHub Spec Kit](https://github.com/github/spec-kit)으로 "명세 → 계획 → 작업 → 구현" 순서로 만들었다.

## 문서

| 위치 | 내용 |
| --- | --- |
| [`specs/001-tistory-blog/spec.md`](specs/001-tistory-blog/spec.md) | 기능명세서 (71개 기능, 기능 ID는 팀 통합 명세서와 같음) |
| [`specs/001-tistory-blog/plan.md`](specs/001-tistory-blog/plan.md) | 설계 계획 (기술 스택, 폴더 구조, 구현 단계) |
| [`specs/001-tistory-blog/research.md`](specs/001-tistory-blog/research.md) | 기술 선택 이유 |
| [`specs/001-tistory-blog/data-model.md`](specs/001-tistory-blog/data-model.md) | 테이블 설계 |
| [`specs/001-tistory-blog/contracts/rest-api.md`](specs/001-tistory-blog/contracts/rest-api.md) | REST API 목록 |
| [`specs/001-tistory-blog/quickstart.md`](specs/001-tistory-blog/quickstart.md) | 실행·확인 순서 |
| [`specs/001-tistory-blog/tasks.md`](specs/001-tistory-blog/tasks.md) | 작업 목록 133개 (기반 → P0 → P1 → P2 순서, 작업마다 기능 ID) |
| [`specs/001-tistory-blog/erd/`](specs/001-tistory-blog/erd/) | ERD 그림 (전체, 1차 범위는 `first-release/`) |
| [`specs/001-tistory-blog/sql/indexes.sql`](specs/001-tistory-blog/sql/indexes.sql) | 인덱스 SQL |
| [`specs/001-tistory-blog/checklists/requirements.md`](specs/001-tistory-blog/checklists/requirements.md) | 명세 품질 체크리스트 |
| [`.specify/memory/constitution.md`](.specify/memory/constitution.md) | 프로젝트 원칙 (모든 단계에서 지킬 규칙) |
| `.specify/templates/`, `.specify/scripts/` | Spec Kit 템플릿과 스크립트 |
| `.claude/skills/speckit-*` | Claude Code에서 쓰는 Spec Kit 명령 |

## Spec Kit 명령 (Claude Code에서 입력)

1. `/speckit-specify` — 기능명세서를 쓰거나 고친다
2. `/speckit-clarify` — 명세에서 애매한 부분을 질문받고 답을 반영한다 (선택)
3. `/speckit-plan` — 설계 계획을 만든다
4. `/speckit-tasks` — 작업 목록을 만든다
5. `/speckit-implement` — 작업 목록 순서대로 구현한다 (코드는 blog-dock에 쓴다)

명세를 고치고 싶으면 `spec.md`를 직접 고치거나 `/speckit-specify`로 다시 써도 된다.

이 문서는 원래 blog-dock 저장소의 `specs/`, `.specify/`, `.claude/skills/`에 있었고, 그때까지의 고친 기록은 blog-dock의 커밋 기록에 남아 있다.
