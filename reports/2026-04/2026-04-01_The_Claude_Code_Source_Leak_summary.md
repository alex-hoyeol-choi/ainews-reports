# The Claude Code Source Leak - 요약

**원문 URL**: https://www.latent.space/p/ainews-the-claude-code-source-leak
**번역일**: 2026-04-01 07:18
**발행일**: 2026-04-01

---

### 🔥 주요 뉴스
**[Claude 코드 소스 유출]** — Anthropic의 Claude 코드베이스 500k LOC가 의도치 않게 유출되어, SOTA 에이전트 하네스 설계에 대한 심층적인 기술적 통찰력을 제공했습니다. 이 유출은 모델 가중치보다는 자율 모드, 메모리 시스템, 계획/검토 플로우 등 오케스트레이션 로직을 노출했습니다.
**[OpenAI 대규모 자금 조달 및 기업 가치 공개]** — OpenAI가 수십억 달러 규모의 자금 조달을 마감하며 $24B ARR(연간 반복 매출)을 달성했고, $3B 투자를 유치하며 ARK Invest ETF에 포함되는 "soft IPO"를 진행했습니다. 이는 전성기 Google/Meta보다 4배 빠른 성장 속도입니다.
**[Claude 코드 유출 관련 보안 위협 발생]** — 유출된 Claude 코드를 악용하려는 공격자들이 color-diff-napi 및 modifiers-napi와 같은 의심스러운 npm 패키지를 빠르게 등록하여, 코드를 컴파일하려는 사용자들에게 실시간 보안 위험을 초래했습니다.

### 🛠️ 제품 & 도구
*   Claude 코드에는 AgentTool, BashTool, FileReadTool 등 20개 미만의 도구(총 60개 이상)가 기본적으로 활성화되어 있습니다.
*   ULTRAPLAN 및 KAIROS를 포함한 직원 전용 게이트 및 TUI 등 여러 미출시/내부 기능들이 개발 중이며, 이 중 일부는 최근 출시되었습니다.
*   내부 MAGIC DOCS가 존재하며, Claude 코드 팀은 /web-setup을 통해 더 쉬운 로컬/웹 GitHub 자격 증명 설정 기능을 발표했습니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/c3642b10-1f7e-490a-af0d-986b24180a1c_1600x1084.png)
![Image](https://substack-post-media.s3.amazonaws.com/public/images/0b39db63-a7b1-48a1-839d-c49812c659e_1773x1822.jpeg)

### 🔬 연구 & 논문
*   Claude의 에이전트 하네스 설계는 컨텍스트에 레포 상태(예: 최근 커밋, git 브랜치 정보)를 포함하고, 적극적인 캐시 재사용 및 커스텀 Grep/Glob/LSP를 활용합니다.
*   Claude의 메모리는 MEMORY.md, 필요에 따라 로드되는 토픽 파일, 검색 가능한 전체 세션 기록의 3계층 설계로 구성되어 있습니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/d5c7ee5f-e03e-434b-b52a-3c0a0470e111_1444x577.png)
![](https://substack-post-media.s3.amazonaws.com/public/images/658d124b-b5d7-4075-af07-2bb850a2d32_1754x1052.png)
*   메모리 병합, 중복 제거, 가지치기, 모순 제거를 위한 "autoDream" 모드가 있으며, mem0의 심층 분석에 따르면 8단계와 5가지 유형의 컴팩션이 있습니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/a4d57d8b-f3b3-4005-90bc-129661d815b_1899x2048.png)
![](https://substack-post-media.s3.amazonaws.com/public/images/0165c08d-6763-490a-9b76-5c9c957f5d06_1182x1612.png)
*   서브에이전트는 KV 캐시를 사용하여 포크-조인 모델을 생성하며, 이는 전체 컨텍스트를 포함하고 작업을 반복할 필요 없이 병렬 처리를 가능하게 합니다.
*   Claude 코드에는 5단계 권한 시스템과 2가지 유형의 계획 모드가 구현되어 있으며, 파일 읽기 중복 제거 및 도구 결과 샘플링 기능도 포함됩니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/9d020dee-d813-4868-8df5-29454d48129a_1254x1592.png)
![Image](https://substack-post-media.s3.amazonaws.com/public/images/59924d12-f74b-4ba8-9272-5419fbad1ecd_1451x1609.jpeg)
*   복원력 및 재시도 메커니즘이 코드에 포함되어 있어 에이전트의 안정적인 작동을 지원합니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/293e920e-2e19-4e16-a04d-c52d699afe6b_1206x1228.png)

### 💰 산업 동향
*   OpenAI는 수십억 달러 규모의 자금 조달을 완료하며 $24B ARR을 달성했고, $3B 투자를 유치하며 ARK Invest ETF에 포함되는 "soft IPO"를 진행했습니다.
*   Anthropic은 유출된 Claude 코드의 재배포를 억제하기 위해 DMCA 테이크다운 조치를 취했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
