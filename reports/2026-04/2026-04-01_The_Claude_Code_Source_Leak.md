# The Claude Code Source Leak

**원문 URL**: https://www.latent.space/p/ainews-the-claude-code-source-leak
**번역일**: 2026-04-01 07:18
**발행일**: 2026-04-01

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Claude 코드 소스 유출

### Claude 코드의 의도치 않은 "오픈소스화"가 수많은 통찰력을 제공합니다.
공유OpenAI의 인류 역사상 최대 규모 자금 조달이 오늘 마감되어 수십억 달러가 추가로 유입되었고, $24B ARR(전성기 Google/Meta보다 4배 빠른 성장)과 같은 멋진 수치들이 공개되었습니다. 또한 부유층으로부터 $3B 투자를 유치하고 ARK Invest의 ETF에 포함되는 "비공개 기업 공개(soft IPO)"도 진행되었습니다. 하지만 ChatGPT WAU 성장은 정체된 것으로 보이며, 2025년 말 목표인 1B WAU를 아직 넘지 못했습니다. Codex 또한 3월에 새로운 이정표를 발표하지 않아 우려를 낳고 있습니다.
오늘의 가장 큰 뉴스는 단연 Claude 코드 소스 유출입니다. Anthropic에게 직접적인 피해는 크지 않지만, 분명 당혹스러우며 동시에 교육적인 사건이었습니다. 코딩 에이전트 덕후들에게는 이른 크리스마스 선물과 같았습니다. 500k LOC 코드베이스를 다루는 수많은 트윗과 게시물을 읽어볼 수 있으며, 소스의 여러 호스팅된 포크를 탐색할 수 있습니다.
전체 동사 목록, Capybara/Mythos v8, /buddy 만우절 기능, Boris의 WTF 카운터 확인, 저주받은 "Claude Codex" 생성, 또는 수십 가지 미출시 기능과 같은 재미있는 흥미거리들이 있지만, 대부분의 진지한 업계 관계자들은 몇 가지 사항에 대해 언급하고 있습니다. Sebastian Raschka는 아마도 상위 6가지 목록을 잘 정리했을 것입니다.
1.  컨텍스트에 레포 상태 넣기 (예: 최근 커밋, git 브랜치 정보)
2.  적극적인 캐시 재사용
3.  커스텀 Grep/Glob/LSP (업계 표준)
Claude 코드에는 기본적으로 20개 미만의 도구(총 60개 이상)가 활성화되어 있습니다: AgentTool, BashTool, FileReadTool, FileEditTool, FileWriteTool, NotebookEditTool, WebFetchTool, WebSearchTool, TodoWriteTool, TaskStopTool, TaskOutputTool, AskUserQuestionTool, SkillTool, EnterPlanModeTool, ExitPlanModeV2Tool, SendMessageTool, BriefTool, ListMcpResourcesTool, ReadMcpResourceTool.
4.  파일 읽기 중복 제거/도구 결과 샘플링
5.  구조화된 세션 메모리 (자세한 내용은 후술)
6.  서브에이전트

![](https://substack-post-media.s3.amazonaws.com/public/images/d5c7ee5f-e03e-434b-b52a-3c0a0470e111_1444x577.png)

## 메모리
Claude 코드의 메모리는 1) 다른 지식으로의 인덱스 역할을 하는 MEMORY.md, 2) 필요에 따라 로드되는 토픽 파일, 3) 검색 가능한 전체 세션 기록의 3계층 설계로 구성되어 있습니다. 또한 메모리 병합, 중복 제거, 가지치기, 모순 제거를 위한 "수면"용 "autoDream" 모드도 있습니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/658d124b-b5d7-4075-af07-2bb850a2d32_1754x1052.png)
mem0의 심층 분석에 따르면 8단계가 있습니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/a4d57d8b-f3b3-4005-90bc-129661d815b_1899x2048.png)
캡션...그리고 5가지 유형의 컴팩션이 있습니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/0165c08d-6763-490a-9b76-5c9c957f5d06_1182x1612.png)

## 서브에이전트는 프롬프트 캐싱을 사용합니다
CC의 핵심 기능: 서브에이전트를 위한 포크-조인 모델을 생성하기 위해 KV 캐시를 사용하며, 이는 전체 컨텍스트를 포함하고 작업을 반복할 필요가 없음을 의미합니다. 즉, 병렬 처리가 기본적으로 무료입니다.

## 5단계 권한 시스템

![](https://substack-post-media.s3.amazonaws.com/public/images/9d020dee-d813-4868-8df5-29454d48129a_1254x1592.png)

## 2가지 유형의 계획 모드
여기:

![Image](https://substack-post-media.s3.amazonaws.com/public/images/59924d12-f74b-4ba8-9272-5419fbad1ecd_1451x1609.jpeg)

## 복원력/재시도

![](https://substack-post-media.s3.amazonaws.com/public/images/293e920e-2e19-4e16-a04d-c52d699afe6b_1206x1228.png)

## 기타 미출시/내부 기능
직원 전용 게이트 및 직원용 TUI를 포함하여 ULTRAPLAN 및 KAIROS를 비롯한 개발 중인 여러 다른 기능들이 있습니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/c3642b10-1f7e-490a-af0d-986b24180a1c_1600x1084.png)
이 중 일부는 [최근 출시되었습니다](https://x.com/himanshustwts/status/2038941583148810701?s=20).
그리고 내부 MAGIC DOCS:

![Image](https://substack-post-media.s3.amazonaws.com/public/images/0b39db63-a7b1-48a1-839d-c498202c659e_1773x1822.jpeg)
> 2026년 3월 23일~3월 24일 AI 뉴스입니다. 12개 서브레딧, 544개 트위터 계정을 확인했으며, 추가 디스코드 채널은 확인하지 않았습니다. AINews 웹사이트에서 모든 지난 호를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
주요 소식: Claude 코드 소스 유출 — 아키텍처 발견, Anthropic의 대응, 경쟁사 반응

## 무슨 일이 있었나
Claude 코드는 배포된 소스 맵 / 패키지 콘텐츠를 통해 상당한 소스 아티팩트가 노출되었고, 이는 신속한 공개 리버스 엔지니어링, 미러링 및 파생 포트를 촉발했습니다. 논의는 빠르게 "당혹스러운 유출"에서 "이것이 SOTA 에이전트 하네스 설계에 대해 무엇을 드러내는가?"로 전환되었습니다. 여러 관찰자들은 이번 유출이 모델 가중치보다는 자율 모드, 메모리 시스템, 계획/검토 플로우, 모델별 제어 로직을 포함한 오케스트레이션 로직을 노출했다고 강조했습니다. 공개 포크가 확산되었고, 한 게시물은 법적 우려로 인해 Codex를 사용한 Python 변환 작업(Yuchenj_UW)으로 이어지기 전에 한 포크가 32.6k 스타와 44.3k 포크를 기록했다고 주장했습니다. 이후 논평에서는 노출된 코드의 양이 500k+ 라인(Yuchenj_UW)이라고 언급했습니다. Anthropic은 여러 게시자(dbreunig, BlancheMinerva)에 따라 DMCA 테이크다운을 통해 재배포를 억제하기 위해 움직였습니다. 별도로, Claude 코드 팀원은 이번 여파 속에서 /web-setup을 통한 더 쉬운 로컬/웹 GitHub 자격 증명 설정(catwu)이라는 제품 기능을 발표했는데, 이는 정상적인 제품 운영이 계속되었음을 암시합니다. 이번 유출은 또한 실시간 보안 위험을 초래했습니다. 공격자들이 유출된 코드를 컴파일하려는 사람들을 표적으로 삼기 위해 color-diff-napi 및 modifiers-napi와 같은 의심스러운 npm 패키지를 빠르게 등록했습니다(Butanium_).

## 사실 대 의견
트윗에서 합리적으로 사실인 내용은 다음과 같습니다.

## 7일 무료 체험으로 계속 읽으세요
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-the-claude-code-source-leak&utm_source=paywall-free-trial&utm_medium=web&utm_content=192814599&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인하세요](https://substack.com/sign-in?redirect=%2Fp%2Fainews-the-claude-code-source-leak&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
