# Anthropic Claude Opus 4.7 - literally one step better than 4.6 in every dimension - 요약

**원문 URL**: https://www.latent.space/p/ainews-anthropic-claude-opus-47-literally
**번역일**: 2026-04-17 06:36
**발행일**: 2026-04-17

---

### 🔥 주요 뉴스
**[Claude Opus 4.7 출시 및 SOTA 성능 달성]** — Anthropic이 최신 Opus 모델인 Claude Opus 4.7을 공식 출시했습니다. 이 모델은 SWE-bench Pro에서 64.3%를 기록하며 이전 4.6 대비 11점 상승했고, GDPval-AA 및 Vals Index에서 1위를 차지하는 등 코딩, 장기 실행 작업, 비전 등 여러 벤치마크에서 SOTA 성능을 보였습니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/7242e5f5-6105-4489-bc8b-143002fe7da6_1344x756.png)
**[향상된 비전 기능 및 고해상도 이미지 지원]** — Opus 4.7은 긴 쪽이 최대 2,576픽셀(약 3.75메가픽셀)의 고해상도 이미지를 지원하며, 이는 이전 Claude 모델보다 3배 이상 큰 크기입니다. 이를 통해 미세한 시각적 디테일에 의존하는 멀티모달 활용 사례가 가능해졌습니다.
**[새로운 토크나이저 도입 및 토큰 경제학 변화]** — Opus 4.7은 새로운 토크나이저를 사용하여 동일 입력에 대해 최대 35% 더 많은 토큰을 사용할 수 있으나, 전반적인 추론 효율성 향상으로 총 토큰 사용량은 이전 모델 대비 최대 50% 감소했습니다. Anthropic은 토큰 사용량 증가를 상쇄하기 위해 모든 구독자의 한도를 늘렸습니다.

### 📊 모델 & 벤치마크
*   Claude Opus 4.7은 SWE-bench Pro에서 64.3%(Opus 4.6 대비 +11점), SWE-bench Verified에서 87.6%(+7점), TerminalBench 2.0에서 69.4%(+4점)를 기록하며 성능이 향상되었습니다.
*   문서 추론 벤치마크에서 80.6%를 달성했으며, GDPval-AA에서 1753 Elo로 새로운 1위를 차지하며 GPT-5.4 대비 약 60%의 승률을 보였습니다.
*   Vals AI는 Opus 4.7이 Vals Index에서 71.4%로 1위를 기록했고, Vibe Code Bench, Vals Multimodal, Finance Agent 등 여러 벤치마크에서도 1위를 차지했다고 발표했습니다.
*   LlamaIndex의 ParseBench 결과에 따르면 Opus 4.7은 차트 이해에서 13.5%에서 55.8%로 크게 개선되었으나, 레이아웃 이해는 16.5%에서 14.0%로 퇴보했습니다.
*   Anthropic은 장문 컨텍스트 평가에서 MRCR 메트릭을 Graphwalks로 대체할 예정이며, Graphwalks에서 Opus 4.6 대비 38.7%에서 58.6%로 성능이 향상되었다고 밝혔습니다.
*   Opus 4.7은 Firefox 셸 익스플로잇과 같은 일부 익스플로잇 관련 평가에서 4.6보다 높은 점수를 기록하며 Mythos에 가까운 프롬프트 인젝션 견고성을 보였습니다.

### 🛠️ 제품 & 도구
*   Claude Opus 4.7은 Claude 플랫폼 및 앱에서 즉시 사용 가능하며, Claude Code는 기본 xhigh 노력 수준을 지원합니다.
*   Anthropic은 공개 베타로 작업 예산 기능을 출시하고, Claude Code에 /ultrareview 기능을 추가하며, Claude Code Max 사용자에게 더 넓은 Auto 모드 접근성을 제공했습니다.
*   새로운 xhigh 추론 노력 모드가 도입되어 high와 max 사이에 위치하며, Claude Code는 Opus 4.7에 대해 기본적으로 xhigh를 사용합니다.
*   Opus 4.7은 긴 쪽이 최대 2,576픽셀(약 3.75MP)인 고해상도 이미지를 지원하여 이전 Claude 모델보다 3배 이상 큰 이미지 입력을 처리할 수 있습니다.

### 🔬 연구 & 논문
*   Opus 4.7은 새로운 토크나이저를 도입하여 토큰 사용량에 변화를 주었으며, 고해상도 이미지 처리 시 더 이상 다운스케일링이 필요 없도록 개선되었습니다.

### 💰 산업 동향
*   Claude Opus 4.7의 백만 입력/출력 토큰당 정가는 $5 / $25로 유지됩니다.
*   Anthropic은 증가된 토큰 사용량을 상쇄하기 위해 모든 구독자의 한도를 늘렸습니다.
*   Anthropic은 학습 중에 사이버 기능을 차등적으로 줄이려는 노력을 실험했다고 시스템 카드에 명시했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
