# Agentic Engineering: WTF Happened in December 2025? - 요약

**원문 URL**: https://news.smol.ai/issues/2026-02-25-wtf-happened
**번역일**: 2026-02-27 05:47
**발행일**: 2026-02-25

---

## AI 산업 브리핑 (2026년 2월 24일~2월 25일)

### 🔥 주요 뉴스

**[Perplexity Computer 출시]** — Perplexity가 파일, 도구, 메모리 및 모델을 오케스트레이션하여 프로젝트를 엔드투엔드로 관리하는 Computer를 출시했습니다. 이는 멀티 모델 라우팅, 샌드박스, 영구 메모리 및 비용 제어를 포함한 시스템 수준 에이전트 UX를 제공하며, Max 구독자에게 먼저 제공되고 사용량 기반으로 가격이 책정됩니다.

**[OpenAI GPT-5.3-Codex 출시 및 가격 공개]** — OpenAI가 API에 GPT-5.3-Codex를 출시했습니다. 이 모델은 약 25% 더 빠른 속도, 작업당 더 적은 토큰, 강력한 SWE-Bench Pro 성능 향상을 주장하며, 입력 토큰당 $1.75, 출력 토큰당 $14의 가격이 책정되었습니다.

**[Anthropic, 책임 있는 스케일링 정책(RSP v3) 변경 및 국방부 압력]** — Anthropic이 "완화 조치가 보장되지 않는 한 임계값을 넘어선 학습 중단"이라는 핵심 안전 서약을 철회하고, 더 빈번한 투명성 아티팩트 및 외부 검토 약속으로 정책을 전환했습니다. 한편, 미국 국방부는 Anthropic에 Claude AI 모델의 안전 가드레일을 제거하고 군사적 사용을 허용할 것을 요구하며, 불이행 시 국방물자생산법(Defense Production Act) 발동 가능성을 경고했습니다.

**[OpenAI 및 Meta, AMD 주식 워런트 확보]** — OpenAI와 Meta가 대규모 미래 GPU 지출과 직접 연결된 주식 리베이트 형태로 총 1억 6천만 AMD 주식에 대한 워런트를 부여받았습니다. 이는 AMD 주가 $600 목표 시 잠재적으로 $1,920억에 달하는 거대한 하드웨어 이면 거래로 평가됩니다.

**[Qwen3.5 Medium 시리즈 출시 및 로컬 에이전트 역량 강화]** — Alibaba가 Qwen3.5 Medium 시리즈(35B-A3B, 27B, 122B-A10B)를 출시하며, 4비트 가중치 및 KV-캐시 양자화에서 "거의 손실 없는" 정확도와 800K~1M 이상의 긴 컨텍스트를 지원합니다. 특히 Qwen3.5-35B-A3B는 로컬 에이전트 루프의 신뢰성을 크게 향상시키며, Qwen3.5-35B-A3B-Base 모델은 오픈소스화되었습니다.

### 📊 모델 & 벤치마크
*   Alibaba Qwen3.5 Medium 시리즈(35B-A3B, 27B, 122B-A10B)가 출시되었으며, 256K 컨텍스트 처리, 에이전틱 코딩, 비전, 채팅에 특화되었습니다.
*   Liquid AI가 240억 파라미터의 스파스 MoE 모델 LFM2-24B-A2B를 출시했으며, 토큰당 20억 파라미터가 활성화되고 32GB RAM에서 실행 가능합니다.
*   Nano Banana 2 (Gemini 3.1 Flash Image)가 출시되어 Pro 버전에 가까운 이미지 품질과 밀집된 구성에서 공간 논리에 탁월하며, 고속/저비용 생산에 적합합니다.
*   Grok-4.20-Beta1이 Search Arena 리더보드에서 1226점으로 1위를 차지하고, Text Arena에서 1492점으로 4위를 기록했습니다.
*   Kimi 2.5가 OS 프론티어 수학 레벨 4 벤치마크에서 4.2%를 기록하여 GLM 5 및 Deepseek V3.2의 두 배 성능을 보였습니다.
*   'Bullshit Benchmark'가 출시되어 AI 모델이 터무니없는 프롬프트를 감지하고 거부하는 능력을 평가하며, Claude Opus 4.6이 높은 성능을 보였습니다.
*   APEX Testing 벤치마크에서 Codex 5.3은 실제 코딩 작업에서 일관되게 좋은 성능을 보인 반면, Qwen 3.5 397B는 복잡한 작업에서 어려움을 겪었습니다.
*   Qwen3.5 Medium 모델이 Text/Vision/Code Arena에 추가되어 직접 비교가 가능해졌습니다.
*   Gemini 3 Pro 이미지 미리보기를 활성화하는 방법이 발견되었으며, 프롬프트 앞에 특정 문구를 추가하여 편집된 이미지를 미리 볼 수 있습니다.
*   Hugging Face에 새로운 Minecraft 플레이 모델인 Andy-4.1이 공개되었습니다.
*   Llama Nemotron Embed VL 1B V2 임베딩 모델이 출시되어 멀티모달 질의응답 리트리벌에 최적화되었습니다.
*   Mercury 2 추론 디퓨전 LLM이 출시되었으며, 기존 속도 최적화 LLM보다 5배 빠르다고 주장됩니다.
*   KREA AI가 저비용 이미지 편집 모델인 Seedream 5 Lite를 출시했습니다.
*   Quiver AI의 첫 모델인 Arrow-1.0이 공개 베타로 출시되어 이미지와 텍스트를 SVG로 변환합니다.

### 🛠️ 제품 & 도구
*   Perplexity Computer가 파일, 도구, 메모리 및 모델을 오케스트레이션하는 엔드투엔드 시스템으로 출시되었습니다.
*   Claude Code가 Slack 플러그인 통합 및 LangSmith 트레이싱을 통한 디버깅 기능을 추가했습니다.
*   GitHub Copilot CLI가 GA(General Availability)를 달성하고, GitHub 코드 검색 기반의 /research 기능을 추가하여 리포지토리 전반의 심층 연구를 지원합니다.
*   Nous Research가 다단계 메모리 시스템과 영구 전용 머신 접근 권한을 갖춘 오픈소스 Hermes Agent 레포를 공개했습니다.
*   OpenPad 앱이 개발 중이며, iPad의 M2 프로세서를 활용하여 로컬 모델로 OpenClaw와 같은 기능을 iPad에서 실행할 수 있도록 합니다.
*   Aider 코딩 어시스턴트가 AI 생성 코드 편집을 즉시 승인하고 실행할 수 있는 /ok 별칭을 메인 브랜치에 병합했습니다.
*   LM Studio 팀이 Tailscale을 래핑하여 로컬 LLM 서버에 대한 원활하고 종단 간 암호화된 원격 접근을 제공하는 LM Link를 출시했습니다.
*   Serenade라는 새로운 구문이 공개되었으며, Python처럼 작성되지만 C++, CUDA 및 x86-64 ASM으로 직접 트랜스파일되며 네이티브 Dear ImGui GUI 지원을 제공합니다.
*   Cloudflare가 Next.js의 대안으로 Vinext 프레임워크를 소개했으며, 트래픽 인식 사전 렌더링을 구현하여 빌드 시간을 단축합니다.
*   Cognition이 Devin 2.2를 출시하며 컴퓨터 사용 기능, 자체 검증 및 자동 수정 기능을 제공하고, 3배 빠른 시작 속도와

---

*이 문서는 news.smol.ai의 뉴스레터를 자동 요약한 것입니다.*
