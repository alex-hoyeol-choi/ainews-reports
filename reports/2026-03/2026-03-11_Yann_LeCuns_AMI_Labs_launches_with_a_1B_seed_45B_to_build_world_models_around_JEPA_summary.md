# Yann LeCun’s AMI Labs launches with a $1B seed @ $4.5B to build world models around JEPA - 요약

**원문 URL**: https://www.latent.space/p/ainews-yann-lecuns-ami-labs-launches
**번역일**: 2026-03-11 12:41
**발행일**: 2026-03-11

---

다음은 바쁜 기술 경영진과 AI 엔지니어를 위한 핵심 AI 뉴스 브리핑입니다.

### 🔥 주요 뉴스
**[Yann LeCun의 AMI Labs, 10.3억 달러 시드 투자 유치하며 출범]** — Yann LeCun이 물리적 세계를 이해하는 JEPA 기반 월드 모델 구축을 목표로 하는 Advanced Machine Intelligence (AMI Labs)를 공식 발표했습니다. 이 스타트업은 35억 달러의 프리머니 가치로 10.3억 달러(8억 9천만 유로)의 시드 투자를 유치하며, 역사상 가장 큰 시드 라운드 중 하나로 기록되었습니다. 프랑스 및 유럽 정치권은 이를 유럽 AI의 주요 이정표로 환영했습니다.

### 📊 모델 & 벤치마크
*   Google은 텍스트, 이미지, 비디오, 오디오, 문서에 대한 단일 임베딩 공간을 제공하는 첫 완전 멀티모달 임베딩 모델인 Gemini Embedding 2를 출시했습니다. 이 모델은 8,192 토큰 텍스트 입력과 100개 이상의 언어를 지원하며, MRL을 통해 3072/1536/768의 출력 차원을 제공합니다.
*   RWKV-7 G1e 모델이 13B, 7B, 3B, 1B 크기로 출시되었습니다.
*   Hume TADA 오픈소스 TTS 모델이 출시되었으며, 1,000개 이상의 테스트 샘플에서 콘텐츠 환각이 없고 유사 LLM-TTS보다 5배 빠르며 2,048 토큰으로 약 700초 오디오를 생성할 수 있습니다.
*   Phi-4-reasoning-vision-15B가 컴팩트한 오픈 멀티모달 모델로 강조되었습니다.
*   Google Sheets에 통합된 Gemini가 SpreadsheetBench에서 70.48%를 달성하여 인간 전문가 수준에 근접한 성능을 보였습니다.
*   Megatron Core MoE가 대규모 MoE 학습을 위한 오픈 프레임워크로 출시되었으며, DeepSeek-V3-685B에 대해 1233 TFLOPS/GPU를 달성했다고 주장했습니다.
*   OfficeQA Pro 벤치마크가 엔터프라이즈 기반 추론을 위해 도입되었으며, 최신 에이전트들의 성능이 여전히 50% 미만임을 보여주었습니다.
*   SWE-bench Verified 벤치마크는 유지보수자들이 평가자를 통과한 에이전트 PR의 약 절반만을 병합한다는 점을 밝혀냈습니다.
*   AuditBench는 정렬 감사 평가를 위해 숨겨진 행동이 이식된 56개의 LLM을 소개했습니다.
*   CodeClash 벤치마크는 장기 코딩 및 계획 능력을 탐색하며, 최고 모델들이 지속적인 에이전트 적대적 환경에서 여전히 저조한 성과를 보임을 보여주었습니다.
*   Google의 AMIE는 응급 진료 워크플로우에 대한 전향적 임상 연구에서 전반적인 감별 진단 및 관리 계획 품질이 PCPs와 유사했지만, PCPs가 실용성과 비용 효율성에서 더 우수하다는 결과를 보고했습니다.

### 🛠️ 제품 & 도구
*   VS Code Agent Hooks가 정책 시행 및 워크플로우 지침을 위해 출시되었습니다.
*   GitHub/Figma MCP(Multi-modal Copilot)가 디자인과 코드 간의 루프를 닫는 기능을 제공합니다.
*   LangGraph deploy 및 LangGraph 1.1이 프로덕션화를 단순화하기 위해 출시되었습니다.
*   Ollama scheduled prompts가 Claude Code에 추가되어 간단한 자동화 루프를 가능하게 합니다.
*   Google Workspace/Gemini 배포가 Docs, Sheets, Slides, Drive 전반으로 확장되었으며, Sheets 작업 9배 가속, AI 생성 슬라이드 레이아웃, Drive 수준의 문서 간 답변 기능이 추가되었습니다.

### 🔬 연구 & 논문
*   Cameron Wolfe는 LLM 평가의 신뢰도를 높이기 위해 95% 신뢰 구간을 보고하는 실용적인 통계 스레드를 게시했습니다.
*   "사고 단계"의 97% 이상이 장식적이며 CoT(Chain-of-Thought) 모니터링이 신뢰할 수 없다는 연구 결과가 발표되었습니다.
*   Baseten과 Harvard의 협력을 통해 인퍼런스 효율성을 위한 프리픽스 캐싱 연구가 진행되었습니다.
*   Karpathy는 코드 편집, 짧은 학습 실행, 지표 기반 유지/폐기 로직을 포함하는 자동 연구(autoresearch) 개념을 제시했습니다.
*   Yuchen Jin은 Claude 기반의 "수석 과학자" 루프를 통해 8개 GPU에서 11시간 이상 568회 실험을 실행하여 자동화된 연구 과정을 시연했습니다.
*   AI 지원을 통한 FrontierMath 미해결 문제 해결 가능성이 제기되었으며, GPT-5.4 Pro가 이를 해결했다고 주장되었습니다.
*   Sharon Zhou는 프로덕션 환경에서 AI 커널 최적화에 대한 초인적인 성능을 주장하며, 자동 GPU 포팅 및 최적화의 실용화 가능성을 시사했습니다.

### 💰 산업 동향
*   Yann LeCun의 AMI Labs는 10.3억 달러의 시드 투자를 유치하며 35억 달러의 프리머니 가치를 인정받았고, 이는 유럽 기업 중 가장 큰 시드 라운드일 가능성이 높습니다.
*   프랑스 대통령 Emmanuel Macron과 Bpifrance는 AMI Labs의 출범을 유럽 AI의 새로운 장이자 프랑스 AI 역량의 중요한 이정표로 환영했습니다.
*   Microsoft는 50만 건 이상의 대화 분석을 기반으로, 2025년 Copilot 모바일 사용자에게 건강이 #1 주제였다고 보고했습니다.

### ⚡ 인프라 & 하드웨어
*   Together MCP 서버 및 Together GPU Clusters가 에이전트 기반 앱 구축 및 스케일을 위한 인프라를 추가했습니다.
*   Hugging Face Storage Buckets가 Xet 중복 제거를 기반으로 구축된 S3와 유사한 가변 스토리지로 출시되었으며, 월 8달러/TB부터 시작합니다.
*   Karpathy는 다중 에이전트 연구 협업을 위한 "에이전트를 위한 GitHub"인 AgentHub를 암시했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
