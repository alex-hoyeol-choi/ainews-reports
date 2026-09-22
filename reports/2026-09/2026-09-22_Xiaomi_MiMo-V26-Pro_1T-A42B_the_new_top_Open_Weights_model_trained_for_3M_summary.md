# Xiaomi MiMo-V2.6-Pro 1T-A42B: the new top Open Weights model, trained for $3M - 요약

**원문 URL**: https://www.latent.space/p/ainews-xiaomi-mimo-v26-pro-1t-a42b
**번역일**: 2026-09-22 07:01
**발행일**: 2026-09-22

---

### 🔥 주요 뉴스
*   **Xiaomi MiMo-V2.6 시리즈 출시:** Xiaomi가 네이티브 옴니모달 오픈 웨이트 모델인 MiMo-V2.6 Pro, Flash, Pro-UltraSpeed를 공개했습니다. MiMo-V2.6 Pro는 Intelligence Index에서 46점을 기록하며 최고 오픈 웨이트 모델로 데뷔했으며, 1.02T/활성 42B 파라미터와 강력한 비용 효율성을 자랑합니다.
    ![X avatar for @ArtificialAnlys](https://pbs.substack.com/profile_images/2042402069320290304/A8C1lP07.jpg)
    ![](https://substack-post-media.s3.amazonaws.com/public/images/e2e1163e-d6ca-41dc-93b6-65900faa37d1_1508x900.png)
*   **OpenAI, 미해결 수학 문제 100개 이상 해결 주장 및 학습 자동화:** OpenAI가 수학 분야 AI 발전을 위한 독립 자문 그룹을 발표하고, 내부 모델이 100개 이상의 오랜 미해결 수학 문제를 해결했다고 주장했습니다. 또한, GPU 커널 작성 및 코드 최적화를 포함한 실험 모델 학습의 상당 부분을 자동화하여 일부 실험 기간을 수년에서 약 일주일로 단축했습니다.
*   **Qwen-Image 2.1 출시 및 라이선스 명확화:** Qwen-Image-2.1 (7B 파라미터)이 오픈 웨이트 통합 이미지 생성/편집 모델로 출시되었습니다. 네이티브 RGBA/투명 이미지 생성 및 편집, 최대 10개의 참조 이미지 지원, 멀티 이미지 인퍼런스 가속 등 새로운 기능을 제공하며, 생성된 출력물에 대한 사용자 권리를 명확히 했습니다.
    ![](https://preview.redd.it/59fu834idoqh1.png?width=767&format=png&auto=webp&s=5fb81b135b35dac70f9d38a9995d7c1a7a2877dd)
    ![](https://preview.redd.it/cvh09tyvdoqh1.jpeg?width=1242&format=pjpg&auto=webp&s=32077f7420def5bec85160e2e982d6aef5efce54)
*   **Jev, 의사결정 모델 생태계 확장:** Jev는 '사고 없음, 단일 토큰, 낮은 레이턴시 허용 가능한 인텔리전스'를 위한 분류/라우팅 모델로 소개되었습니다. LangChain이 Jev를 LangSmith에 심판으로 추가하고, 오픈소스 의사결정 모델 SemIf가 LangSmith Gateway를 통해 푸시되는 등 생태계가 빠르게 확장되고 있습니다.

### 📊 모델 & 벤치마크
*   Xiaomi MiMo-V2.6 Pro는 Intelligence Index에서 46점을 기록하며 최고 오픈 웨이트 모델로 데뷔했으며, 총 1.02T / 활성 42B 파라미터를 가집니다.
*   Grok 4.7이 SpaceXAI에 의해 출시되었으며, Grok 4.6 대비 개선되었다고 설명됩니다. Artificial Analysis는 Coding Agent Index에서 56점을 기록하며 개선을 보였으나, Vals Index에서는 24위로 5점 하락했습니다.
*   Qwen-Image-2.1 (7B 파라미터)은 오픈 웨이트 통합 이미지 생성/편집 모델로 출시되었으며, 이전 Qwen 이미지 모델보다 상당히 작아 로컬 인퍼런스에 적합합니다.

### 🛠️ 제품 & 도구
*   Xiaomi는 RL 환경 및 학습 레시피를 오픈소스화할 예정이며, 코딩, 사이버, 일반, 시각, 음악 생성 등 다양한 다중 작업 학습 스위트를 포함합니다.
*   Hugging Face Tokenizers v1 RC가 출시되어 최대 30배 빠른 토큰화, 개선된 멀티스레드 스케일링, 낮은 메모리 사용량 및 작은 패키지 크기를 제공합니다.
*   Halo는 모델을 네이티브 Hugging Face 형식으로 유지하면서 기본 TRL 대비 최대 2.8배의 처리량을 주장하는 후처리 프레임워크로 출시되었습니다.
*   Cognition은 Devin Cloud를 Terminal 및 devin ssh에 도입하여 모델의 VM이 CLI에서 직접 접근 가능하도록 하고, Devin과 사용자 머신 간의 핸드오프를 허용했습니다.
*   GitHub Copilot은 데스크톱 앱에서 편집 가능한 diff를 예고했으며, Sentry는 크래시 리포트에서 수정으로 이동하기 위한 통합 캔버스를 선보였습니다.
*   Parakeet Redux는 NVIDIA의 음성 모델을 1.2GB에서 178MB로 압축하고 CPU에서 실시간의 113배 속도로 실행되며, 25개 언어 FLEURS에서 기본 모델을 능가합니다.

### 🔬 연구 & 논문
*   Xiaomi는 기술 보고서에서 더 큰 배치와 높은 처리량, 더 많은 작업과 풍부한 환경, 더 많은 그레이더 컴퓨팅을 통해 RL 컴퓨팅을 스케일링하는 세 가지 축을 언급했습니다.
    ![](https://substack-post-media.s3.amazonaws.com/public/images/af7a24ce-df99-410f-85ef-d4f83c7649c3_1542x818.png)
*   OpenAI는 수학 분야 AI 발전의 평가 및 소통을 안내하기 위해 수학자들로 구성된 독립 자문 그룹을 발표했습니다.
*   Eidon AI는 1,274시간의 자기 중심 로봇 공학 데이터(13,451개 기록)를 오픈소스화했습니다.

### 💰 산업 동향
*   중국 랩들은 Kimi K3, Qwen3.8-Max, DeepSeek V4-Pro, GLM-5.3, Hy4 Preview, Atria Dawn 등 약 10주간 이례적으로 집중된 오픈 모델 릴리스를 선보였습니다.
*   Bloomberg는 스타트업들이 비용 절감 및 OpenAI/Anthropic 의존도 감소를 위해 오픈 웨이트 기반 커스텀 모델 구축 경향이 증가하고 있다고 보도했습니다.
*   Qwen-Image-2.1 개발자들은 모델 출력이 라이선스된 "Materials"로 간주되지 않아 사용자가 생성된 이미지/콘텐츠에 대한 권리를 유지한다고 명확히 했습니다.

### ⚡ 인프라 & 하드웨어
*   Xiaomi의 RL 실행은 130시간, 75B 토큰, 260만 달러가 소요되었으며, JAX + TPU에서 RL을 스케일링했습니다.
*   vLLM은 GB300 NVL72에서 Qwen3.8-2.4T를 위한 튜닝된 서빙 구성을 발표했으며, 높은 처리량에서 GPU당 총 5K 토큰/초에서 낮은 레이턴시에서 사용자당 180 출력 토큰/초까지의 파레토 프론티어를 보여주었습니다.
*   vLLM은 PyNvVideoCodec/NVDEC를 통합하여 CPU 디코딩 병목 현상을 제거하고 8×H100에서 비디오 워크로드 처리량을 2배 이상 향상시켰습니다.
*   Tencent Hunyuan은 Hy4 Preview (770B)를 214 GiB로 패킹하는 데 필요한 엔지니어링을 요약했으며, 이는 패치된 llama.cpp의 커스텀 CUDA 커널을 포함하여 가중치당 평균 약 2.38비트의 혼합 정밀도 양자화를 통해 이루어졌습니다.
*   Patrick Wardle은 Muse의 심각한 로컬 하이재킹 결함을 보고하며, 광범위한 OS 접근이 이러한 어시스턴트를 고가치 공격 표면으로 만든다고 주장했습니다.
*   SGLang은 모델 스왑 및 재시작 시 KV 캐시를 보존하기 위한 다단계 hiCache (GPU/RAM/디스크)를 도입했습니다.

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 요약한 것입니다.*
