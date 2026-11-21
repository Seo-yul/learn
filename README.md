# learn

AI Agent와 그 주변 기술을 공부하며 정리한 학습 자료다. GitHub Pages로 배포한다.

- 사이트: https://devops.ai.kr/learn/

| 위치 | 내용 |
|---|---|
| [rag-1.html](rag-1.html), [rag-2.html](rag-2.html) | RAG 1부와 2부: 임베딩, 청킹, 검색, 재순위, 질의 변환, 실패 진단, 평가 |
| [eval-intro.html](eval-intro.html) | Agent 평가(eval) 입문 |
| [oauth/](oauth/index.html) | MCP 서버의 OAuth 6편: role과 scope, JWKS와 introspection, JWT, ID-JAG |
| [toolhive/](toolhive/index.html) | ToolHive 10편과 agentgateway 비교 |
| [aws/](aws/eks-access.html) | EKS 클러스터 접속 |

## 문서 형식

모든 페이지는 `assets/learn.css` 하나를 쓴다. 페이지 안에 `<style>`이나 inline style을 두지 않는다. 문서 머리말의 첫 줄(시리즈와 작성일)은 `<p class="kicker">`로 쓴다.

- 문체는 한다체로 쓰고, 제목은 번호를 붙인 평범한 명사구로 쓴다.
- 회사 환경을 알 수 있는 식별자(호스트명, 저장소 이름, 계정 ID, 클러스터 이름)는 쓰지 않는다.
- 본문에서 쓰는 class는 다음과 같다.

| class | 용도 |
|---|---|
| `box key` | 한 문장 요약처럼 먼저 읽을 내용 |
| `box`, `box warn`, `box ok` | 보충 설명, 주의, 확인된 내용 |
| `label` | 상자의 작은 제목 |
| `tbl` | 표를 감싸는 가로 스크롤 영역 |
| `fig`, `fig flow` | 그림과 캡션. 넓은 그림은 `scroll`로 감싼다. SVG 색은 `d-*` class로 정하고, `s-*`와 `am-*`는 예전 그림에 남아 있는 같은 용도의 class다 |
| `legend`, `note` | 그림 범례와 작은 보충 설명 |
| `lvl l1`, `lvl l2`, `lvl l3` | 초급, 중급, 고급 표시 |
| `th-col`, `ag-col` | 비교 표에서 두 대상의 열 강조 |
| `toc` | 문서 안 목차 |
| `pager` | 시리즈의 이전 글과 다음 글 |
| `entries` | 홈 화면의 문서 목록 |

## 페이지 추가

1. 기존 페이지 하나를 복사해서 영문 파일명으로 저장한다. 시리즈는 폴더를 만들고 `index.html`을 목차로 둔다.
2. `index.html`의 목록에 링크를 한 줄 추가한다.
3. `main`에 push하면 배포된다.
