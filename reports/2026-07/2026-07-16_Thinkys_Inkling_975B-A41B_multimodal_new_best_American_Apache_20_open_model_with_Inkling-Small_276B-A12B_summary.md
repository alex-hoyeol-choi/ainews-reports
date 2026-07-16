# Thinky's Inkling: 975B-A41B multimodal, new best American Apache 2.0 open model (with Inkling-Small, 276B-A12B) - 요약

**원문 URL**: https://www.latent.space/p/ainews-thinkys-inkling-975b-a41b
**번역일**: 2026-07-16 06:53
**발행일**: 2026-07-16

---

다음은 AI 뉴스레터에서 추출한 핵심 신규 소식 요약 브리핑입니다.

### 🔥 주요 뉴스
**Thinking Machines Lab, 첫 오픈 웨이트 멀티모달 LLM 'Inkling' 출시** — 전 OpenAI 리더들이 설립한 TML이 총 975B 파라미터, 활성 41B 파라미터의 Mixture-of-Experts (MoE) 모델 Inkling을 Apache 2.0 라이선스로 공개했습니다. 텍스트, 이미지, 오디오를 네이티브로 추론하며 최대 1M 토큰 컨텍스트 윈도우를 지원합니다.
![](https://substack-post-media.s3.amazonaws.com/public/images/90048da3-a87f-44d8-8ad4-e954031d2721_2540x1692.png)
**Inkling, 미국 오픈 웨이트 모델 중 최고 성능 기록** — Artificial Analysis의 Intelligence Index에서 41점을 기록하며 Nemotron 3 Ultra (38점) 등을 제치고 미국 기반 오픈 웨이트 모델 중 선두에 올랐습니다. Agentic Web App Arena에서도 ELO 1257점으로 9위를 차지하며 Claude Opus 4.6 및 Gemini 3.5 Flash와 유사한 성능을 보였습니다.
**광범위한 인퍼런스 에코시스템, 출시 당일 Inkling 지원** — vLLM, SGLang, Modal, Baseten, Databricks, Hugging Face 등 주요 인퍼런스 스택 및 파트너들이 Inkling 출시 당일부터 NVFP4 및 BF16 지원을 포함한 최적화된 서비스를 제공합니다. 특히 Modal은 커스텀 DFlash 스페큘레이터를 통해 67% 높은 처리량을 달성했습니다.

### 📊 모델 & 벤치마크
*   Thinking Machines Lab은 총 975B 파라미터, 활성 41B 파라미터의 Mixture-of-Experts (MoE) 멀티모달 LLM 'Inkling'을 Apache 2.0 라이선스로 출시했습니다.
*   Inkling은 텍스트, 이미지, 오디오 입력을 지원하며 텍스트를 출력하고, 오픈 웨이트 체크포인트는 최대 1M 토큰의 컨텍스트 윈도우를 지원합니다.
*   Inkling-Small 모델도 함께 공개되었으며, 총 276B 파라미터, 활성 12B 파라미터로 더 낮은 비용과 레이턴시로 강력한 성능을 제공합니다.
*   Artificial Analysis의 Intelligence Index에서 41점을 기록하여 Nemotron 3 Ultra (38점)를 능가하는 선두적인 미국 오픈 웨이트 모델로 평가받았습니다.
*   Agentic Web App Arena에서 ELO 1257점으로 전체 9위를 기록하며, 에이전틱 워크로드에서 가장 높은 순위를 기록한 미국 기반 오픈 웨이트 모델이 되었습니다.
*   GDPval-AA v2 ELO 1238점, τ³-Banking 24%를 기록하여 Kimi K2.6 및 DeepSeek v4 Flash max보다 높은 성능을 보였습니다.

### 🛠️ 제품 & 도구
*   Thinking Machines의 Tinker 플랫폼 및 Playground에서 Inkling 모델을 즉시 지원하며, 당일 파인튜닝이 가능합니다.
*   Tinker API는 64K 컨텍스트 기준 입력 1M당 $1.87, 출력 $4.68, 256K 컨텍스트 기준 입력 1M당 $3.74, 출력 $9.36의 가격 정책을 제공합니다.
*   Unsloth는 Inkling의 1비트 GGUF 양자화 모델을 출시하여, 원본 대비 86% 작은 270GB 크기로 74.2%의 정확도를 유지하며 비전 및 오디오를 지원합니다.

### 🔬 연구 & 논문
*   Inkling은 45조 개의 텍스트, 이미지, 오디오, 비디오 토큰으로 처음부터 사전 학습되었습니다.
*   아키텍처는 5:1의 로컬-글로벌 레이어 비율과 512 윈도우 크기를 가진 하이브리드/슬라이딩 윈도우 어텐션을 사용합니다.
*   RoPE 대신 상대적 위치 인코딩/상대적 어텐션 바이어스를 채택했으며, 어텐션/FFN 스트림 주변에 짧은 컨볼루션 레이어를 추가했습니다.
*   MoE 아키텍처는 2개의 공유 전문가를 포함하며, DeepSeek 스타일의 보조 손실 없는 로드 밸런싱을 적용했습니다.
*   muP 및 Muon/가중치 감쇠 변형(MuonC/AdamC)을 사용한 것으로 확인되었습니다.

### 💰 산업 동향
*   Thinking Machines Lab은 전 OpenAI 리더 및 연구원들이 설립한 회사로, Inkling 출시는 이들의 첫 번째 주요 공개 모델입니다.
*   Inkling은 Tinker, Hugging Face, Databricks, Baseten, Modal, vLLM/SGLang 스택을 통해 광범위하게 이용 가능합니다.

### ⚡ 인프라 & 하드웨어
*   NVIDIA는 Inkling이 GB300 NVL72에서 학습되었으며, NVFP4 체크포인트가 출시 당일 Hugging Face에서 제공되었다고 발표했습니다.
*   vLLM은 Inkling에 대해 NVFP4 및 BF16을 지원하며, Blackwell 및 Hopper에 최적화되어 4× GB200에서 MTP를 사용하여 사용자당 최대 380 tok/s를 달성합니다.
*   Inferact는 sconv 인식 텐서 병렬 샤딩, 저 레이턴시 퓨즈드 콜렉티브, TML의 FA4 sheared-bias 커널 직접 통합 등 시스템 최적화 작업을 상세히 설명했습니다.
*   Modal은 Inkling에 커스텀 DFlash 스페큘레이터를 사용하여 67% 더 높은 처리량과 상호작용성을 제공합니다.
*   LMSYS/SGLang은 ShortConv, 상대적 위치 어텐션, 공유 전문가 싱크 MoE 등 Inkling 아키텍처에 대한 네이티브 지원을 구현했습니다.
*   Lysandre는 TML의 causal Conv1D를 causal-conv1d로, 어텐션을 FlashAttention-4로 교체하여 재학습 없이 총 처리량 약 15% 증가를 달성했다고 보고했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
