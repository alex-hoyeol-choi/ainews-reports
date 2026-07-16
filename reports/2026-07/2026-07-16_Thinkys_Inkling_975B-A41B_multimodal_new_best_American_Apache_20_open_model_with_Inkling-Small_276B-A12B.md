# Thinky's Inkling: 975B-A41B multimodal, new best American Apache 2.0 open model (with Inkling-Small, 276B-A12B)

**원문 URL**: https://www.latent.space/p/ainews-thinkys-inkling-975b-a41b
**번역일**: 2026-07-16 06:53
**발행일**: 2026-07-16

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Thinky의 Inkling: 975B-A41B 멀티모달, 새로운 최고의 미국 Apache 2.0 오픈 모델 (Inkling-Small, 276B-A12B 포함)

### Thinky의 첫 번째 풀 LLM 출시는 대단하며, 게다가 오픈 웨이트 모델입니다!
ShareThinky는 몇 달에 한 번씩만 모습을 드러내는 것 같습니다. 가장 최근에는 Interaction 모델로 나타났지만, 매번 뛰어난 안목과 깊이를 보여주며 깊은 인상을 남깁니다. 오늘 Thinky는 Inkling을 소개했습니다. SOTA 모델은 아니지만, 미국 오픈 모델의 기준이 될 만한 매우 견고한 새 모델 패밀리입니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/90048da3-a87f-44d8-8ad4-e954031d2721_2540x1692.png)
- Inkling이라는 저희 모델은 총 975B 파라미터와 41B 활성 파라미터를 가진 Mixture-of-Experts 트랜스포머입니다.
- 최대 1M 토큰의 컨텍스트 윈도우를 지원합니다.
- 45조 개의 텍스트, 이미지, 오디오, 비디오 토큰으로 사전 학습되었습니다.
- 이 모델은 다양한 크기의 모델 패밀리 중 첫 번째입니다. 이와 함께 Inkling-Small의 프리뷰를 공유합니다. Inkling-Small은 12B 활성 파라미터를 가진 경량 모델로, 유사한 레시피로 학습되었으며 더 낮은 비용과 레이턴시로 강력한 성능을 달성합니다.
- Inkling은 텍스트, 이미지, 오디오에 대해 네이티브로 추론하며, 효율적이고 제어 가능한 사고 노력을 통해 비용과 성능의 균형을 맞춥니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/7f9ce249-0d32-4168-a4c4-9b794019fc74_1620x1628.png)
Hugging Face의 분석은 몇 가지 흥미로운 기술적 특징을 다룹니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/866e482a-de86-43e7-b497-b43f0da8a037_1610x1808.png)
> 2026년 7월 14일~7월 15일 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터 계정을 확인했으며, 추가 Discord는 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI Twitter 요약

## 무슨 일이 있었나
Thinking Machines Lab은 Inkling을 첫 번째 완전 출시 오픈 웨이트 파운데이션 모델 패밀리 엔트리로 선보이며, 벤치마크 최고 성능을 목표로 하는 플래그십 모델이라기보다는 커스터마이징 가능한 멀티모달 베이스 모델로 포지셔닝했습니다.
- Thinking Machines는 Inkling을 "텍스트, 이미지, 오디오 모달리티 전반에 걸쳐 효율적으로 추론하는" 오픈 웨이트 모델로 발표했으며, 전체 웨이트가 제공되고 Tinker 플랫폼 및 Playground @thinkymachines에서 즉시 지원됩니다.
- Mira Murati는 Inkling을 회사의 "첫 모델"이자 "처음부터 학습된" 오픈 웨이트 모델로 설명했으며, Tinker @miramurati에서 당일 파인튜닝이 가능하다고 언급했습니다.
- Soumith Chintala는 Inkling을 Thinking Machines의 "첫 범용 모델"로 규정하며, 오픈 웨이트, 975B 파라미터, 네이티브 멀티모달리티, Tinker, Hugging Face 및 파트너를 통한 가용성을 강조했습니다 @soumithchintala.
- John Schulman은 타임라인 관련 맥락을 덧붙였습니다. 사전 학습은 지난겨울에 시작되었고, 1월 중순부터 소규모 팀이 그 위에 코딩, 추론, 에이전틱 학습을 구축했습니다 @johnschulman2.
- Lilian Weng은 Inkling을 "광범위한 기능 범주에서 견고한 성능"을 목표로 하며 실제 사용 및 커스터마이징을 위한 파운데이션 모델로 특징지었습니다 @lilianweng.
- TML 직원들은 Inkling이 최종 프론티어 모델이라기보다는 향후 반복을 위한 기반이자 출시 첫날의 모델임을 반복적으로 강조했습니다 @soumithchintala, @cHHillee, @keirp1.
- 이번 출시는 vLLM, SGLang, Modal, Baseten, Databricks, Hugging Face, 그리고 양자화/커뮤니티 툴링 전반에 걸쳐 이례적으로 광범위한 출시 당일 에코시스템 지원을 받았습니다 @vllm_project, @lmsysorg, @modal, @baseten, @Yuchenj_UW, @huggingface, @danielhanchen.
- 독립적인 논평가들은 즉시 Inkling을 현재까지 미국 기반 오픈 웨이트 모델 중 가장 강력한 출시작으로 평가했지만, 일부 벤치마크에서는 여전히 최고 수준의 중국 오픈 웨이트 모델 및 최고 성능의 클로즈드 모델에 뒤처진다고 보았습니다 @natolambert, @ArtificialAnlys, @scaling01.

## 핵심 사실 및 사양

### 모델 크기, 모달리티, 라이선스, 컨텍스트
- Inkling은 대부분의 게시물에서 총 975B 파라미터 / 41B 활성 파라미터로 보고되었습니다 @soumithchintala, @vllm_project, @ArtificialAnlys, @kimmonismus. 한 트윗에서는 974B @Yuchenj_UW, 다른 트윗에서는 952B @multimodalart라고 언급했지만, 트윗 세트의 압도적인 합의는 약 975B입니다.
- 토큰당 41B 활성 파라미터를 가진 Mixture-of-Experts 모델입니다 @VictoriaLinML.
- 다수의 반응과 요약에 따르면 Apache 2.0 라이선스를 따릅니다 @natolambert, @Yuchenj_UW, @multimodalart.
- 텍스트, 이미지, 오디오 입력을 지원하며 텍스트를 출력합니다 @soumithchintala, @TheRundownAI, @ArtificialAnlys.
- 오픈 웨이트 체크포인트는 최대 1M 컨텍스트를 지원합니다 @vllm_project, @lmsysorg, @ArtificialAnlys.
- Tinker/API 컨텍스트는 256K로 설명되며, 64K 및 256K 컨텍스트에 따라 가격이 차등화됩니다 @ArtificialAnlys.

### 학습 및 출시 세부 정보
- TML은 Inkling이 처음부터 학습되었다고 말합니다 @miramurati, @LiorOnAI.
- 커뮤니티 독자들은 출시 자료에서 45조 개의 학습 토큰을 추출했지만 @eliebakouch, @ArtificialAnlys, 한 게시물에서는 48조 개라고 언급했습니다 @mervenoyann. 이 데이터 세트에서 더 반복된 수치는 45조 개입니다.
- Inkling은 제어 가능한 추론 노력 / 수치적 노력 수준을 포함합니다 @LiorOnAI, @TheRundownAI, @danielhanchen.
- Tinker 고객들은 최대치의 순수 벤치마크 추구보다는 간결한 추론과 강력한 툴 호출에 중점을 두었습니다 @tinkerapi, @MichaelElabd.

### 반응에서 드러난 아키텍처 세부 정보
몇몇 기술에 정통한 반응들은 출시에서 아키텍처 선택 사항을 추출했습니다.
- 5:1의 로컬-글로벌 레이어 비율과 512의 윈도우 크기를 가진 하이브리드/슬라이딩 윈도우 어텐션 @eliebakouch, @ariG23498.
- RoPE 대신 상대적 위치 인코딩 / 상대적 어텐션 바이어스; 여러 게시자는 이를 가장 혁신적인 대규모 선택 중 하나로 꼽았습니다 @stochasticchasm, @eliebakouch, @rasbt, @arohan, @ChangJonathanC.
- 어텐션/FFN 스트림 주변에 추가된 짧은 컨볼루션 레이어; 논평가들은 이를 짧은 컨볼루션의 이례적인 스케일업 사용으로 지적했습니다 @eliebakouch, @stochasticchasm, @rasbt, @SonglinYang4.
- 공유 전문가 싱크 / 2개의 공유 전문가를 가진 MoE로, 최근 많은 MoE가 1개의 공유 전문가를 사용하는 것과 달리 이례적인 것으로 언급되었습니다 @eliebakouch, @ariG23498.
- 아키텍처에 대한 커뮤니티 분석에서 DeepSeek 스타일의 보조 손실 없는 로드 밸런싱이 언급되었습니다 @eliebakouch.
- muP 및 Muon/가중치 감쇠 변형은 보고서에서 추론되었고 옵티마이저 전문가의 반응으로 확인되었습니다. Aaron Defazio는 그들이 자신의 수정된 가중치 감쇠 접근 방식인 "MuonC/AdamC"를 사용하고 있다고 말했으며 @aaron_defazio, 커뮤니티 독자들은 muP도 지적했습니다 @stochasticchasm, @Laz4rz.
- vLLM은 추측 디코딩을 위한 8개의 MTP 헤드를 강조했습니다 @vllm_project.

### 변형 모델
- Inkling-Small은 예정되거나 별도로 논의된 소형 모델로 반복적으로 언급됩니다 @LiorOnAI, @teortaxesTex.
- 커뮤니티 요약에 따르면 Inkling-Small은 총 276B / 활성 12B 파라미터이며, 여러 평가에서 더 큰 모델에 비해 예상외로 경쟁력이 있다고 설명합니다 @eliebakouch, @nrehiew_.

## 성능 및 벤치마크

### 독립 벤치마크 평가
- Artificial Analysis는 Inkling이 Intelligence Index에서 41점으로 데뷔하여, Nemotron 3 Ultra (38), Gemma 4 31B (29), gpt-oss-120b (24)를 앞서는 선두적인 미국 오픈 웨이트 출시작이 되었다고 말했습니다 @ArtificialAnlys.
- Artificial Analysis는 또한 Inkling이 Intelligence Index 작업당 평균 25K 출력 토큰을 생성하며, GLM-5.2 max의 43K, Kimi K2.6의 38K, DeepSeek v4 Pro max의 37K와 비교하여 상대적으로 토큰 효율적이라고 평가했습니다 @ArtificialAnlys.
- Natolambert는 Inkling을 "Nemotron Ultra보다 확실히 한 단계 발전한" "새로운 최고의 미국 모델"이라고 불렀지만, "에이전틱 벤치에서는 GLM 5.2에, 멀티모달에서는 Kimi K 2.6에 약간 뒤처진다"고 덧붙였습니다 @natolambert.
- Design Arena는 Inkling이 Agentic Web App Arena에서 전체 9위, ELO 1257점을 기록하며 Claude Opus 4.6 및 Gemini 3.5 Flash와 같은 대역에 진입했으며, 에이전틱 워크로드에서 가장 높은 순위를 기록한 미국 기반 오픈 웨이트 모델이라고 평가했습니다 @DesignArena.
- Arena는 출시 당일 Agent Arena / Text / Vision / Code Arena에 Inkling을 추가했습니다 @arena.

### 인용된 특정 벤치마크 수치
Artificial Analysis에서:
- GDPval-AA v2 ELO 1238로, Kimi K2.6 (1190) 및 DeepSeek v4 Flash max (1189)보다 높습니다 @ArtificialAnlys.
- τ³-Banking 24%로, Kimi K2.6 (21%)보다 높고 DeepSeek v4 Flash max (23%)보다 약간 높습니다 @ArtificialAnlys.

### 정성적 성능 평가
긍정적:
- "명확하고 간결한" 추론, 장황하지 않습니다 @MichaelElabd.
- 에이전틱 작업에서 강력한 툴 호출 및 우수한 장기 오류 복구 능력을 보여줍니다 @MichaelElabd.
- 좋은 "사고의 질" / 아첨하지 않는 특성 @skirano, @tinkerapi.
- Alex Kirillov는 Inkling이 많은 옴니 모델에서 보이는 일반적인 "오디오 입력 = 지능 페널티"를 피한다고 주장했지만, 다른 사용자는 더 강력한 뒷받침 증거와 벤치마크를 요청했습니다 @alex_kirillov, @giffmana, @alex_kirillov.
혼합/비판적:
- Scaling01은 벤치마크가 "그리 좋지 않다"고 주장하며, Inkling을 대략 "또 다른 Kimi-K2.6" 수준이며 모든 클로즈드 모델과 GLM-5.2에 뒤처진다고 설명했습니다. Kimi-K3 및 DeepSeek-V4-GA보다 앞서 출시 시기를 조정한 것일 수 있다고 추측했습니다 @scaling01.
- Stochasticchasm은 "멀티모달에는 매우 강력"하지만 "터미널 벤치 등에는 아주 강력하지 않다"고 말했습니다 @stochasticchasm.
- JJitsev는 "증류 없이 학습된 유일한 오픈 웨이트 모델"이라는 과대광고에 반박하며, Inkling은 오픈 웨이트에서 증류를 사용하며 TerminalBench 스타일 평가에서 GLM 5.2보다 성능이 떨어진다고 말했습니다 @JJitsev.
- TeortaxesTex는 역설적인 긍정적 해석을 제시했습니다. 평범한 벤치마크 최고 성능은 실제로는 꼼수/증류 오염이 적고 더 독립적인 데이터 파이프라인을 시사할 수 있다고 보았습니다 @teortaxesTex.

## 인퍼런스, 시스템 및 출시 에코시스템

### 공식 및 파트너 인프라 사실
- NVIDIA는 Inkling이 GB300 NVL72에서 학습되었으며, NVFP4 체크포인트가 출시 당일 Hugging Face에서 제공되었다고 말했습니다 @NVIDIAAI.
- vLLM은 출시 당일 지원에는 NVFP4 및 BF16이 포함되며, Blackwell 및 Hopper에 최적화되어 4× GB200에서 MTP를 사용하여 사용자당 최대 380 tok/s를 달성한다고 말했습니다 @vllm_project.
- Inferact는 시스템 작업을 상세히 설명했습니다: sconv 인식 텐서 병렬 샤딩, 저 레이턴시 퓨즈드 콜렉티브 (bs=1에서 5배 빠름), TML의 FA4 sheared-bias 커널 직접 통합 @inferact.
- LMSYS/SGLang은 Inkling 아키텍처 지원이 ShortConv, 상대적 위치 어텐션, 공유 전문가 싱크 MoE, 프리필 풀 CUDA 그래프, MXFP8 KV 캐시, 커스터마이징된 Megatron 백엔드의 전체 파라미터 및 LoRA RL, 라우팅 리플레이, 크로스-런타임 파라미터 동기화, Modal의 DFlash 추측 디코딩을 포함하여 네이티브로 구현되었다고 말했습니다 @lmsysorg.
- Modal은 Modal의 Inkling이 67% 더 높은 처리량과 상호작용성을 위한 커스텀 DFlash 스페큘레이터를 사용한다고 말했습니다 @modal.
- Soumith Chintala는 Modal의 DFlash 스페큘레이터가 "MTP보다 훨씬 빠르다"고 별도로 강조했습니다 @soumithchintala.

### 커뮤니티 최적화 관찰
- Lysandre는 TML의 인과적 Conv1D를 causal-conv1d로 교체하여 토큰/초당 4% 증가를, 어텐션을 FlashAttention-4로 교체하여 추가로 11% 증가를 달성하여 재학습 없이 총 처리량 약 15% 증가를 가져왔다고 보고했습니다 @LysandreJik.
- Unsloth는 1비트 GGUF 양자화 모델을 출시했으며, 이는 86% 더 작으면서 (270GB 대 1.9TB) 상위 1% 정확도의 74.2%를 유지하며 비전 및 오디오를 지원한다고 합니다 @danielhanchen.

## 가격 및 가용성
- Artificial Analysis는 Tinker 가격을 다음과 같이 명시했습니다.
64K 컨텍스트: 입력 1M당 $1.87, 캐시됨 $0.374, 출력 $4.68
256K 컨텍스트: 입력 1M당 $3.74, 캐시됨 $0.748, 출력 $9.36
@ArtificialAnlys
- Tinker, Hugging Face에서 제공되며, Databricks, Baseten, Modal, vLLM/SGLang 스택을 포함한 출시 파트너를 통해서도 이용 가능합니다 @soumithchintala, @Yuchenj_UW, @baseten, @modal.

## 사실 대 의견

### 출시 및 파트너에 의해 직접 뒷받침되는 사실적 주장
- 오픈 웨이트/전체 웨이트 출시 @thinkymachines.
- 처음부터 학습됨 @miramurati.
- 975B 총 / 41B 활성 MoE, 멀티모달 텍스트-이미지-오디오 입력, 웨이트에서 1M 컨텍스트, Tinker/API에서 256K 컨텍스트 @soumithchintala, @ArtificialAnlys.
- Apache 2.0 라이선스 @natolambert, @Yuchenj_UW.
- 사전 학습은 지난겨울에 시작되었고, 에이전틱/코딩/추론 작업은 1월 중순에 시작되었습니다 @johnschulman2.
- 주요 서빙 스택에서 출시 당일 지원되며, vLLM/Inferact/Modal/NVIDIA로부터 구체적인 성능 주장이 있습니다 @vllm_project, @inferact, @modal, @NVIDIAAI.

### 해석 및 의견
- "최고의 미국 오픈 모델" / "미국 오픈소스 프론티어를 구했다"는 평가는 비록 여러 존경받는 관찰자들에 의해 반복되었지만, 판단에 불과합니다 @natolambert, @karinanguyen, @saranormous.
- Inkling이 OpenAI/Anthropic에서 증류되지 않았기 때문에 특히 중요하다는 주장은 논란의 여지가 있습니다. Jxmnop는 그러한 증류 없이 "유일한 오픈 웨이트 모델"이라고 불렀다가 @jxmnop, 부분적으로 철회했습니다: "분명히 증류를 했지만, 아주 조금만 했다고 합니다 lol." @jxmnop. Andrew Carr 또한 SFT 트레이스에 Kimi 2.5를 사용했음을 지적하며 순수성 프레이밍에 이의를 제기했습니다 @andrew_n_carr.
- Inkling이 중국 모델 출시보다 "서둘러" 출시되었다는 주장은 비평가들의 추측이며, 출시 자료에 의해 입증되지 않습니다 @scaling01.
- 상대적 어텐션이 역전파가 어렵기 때문에 TML에 파인튜닝 해자를 제공한다는 주장은 추측에 불과합니다 @typedfemale.
- Inkling이 멀티모달 지능 손실을 피한다는 주장은 유망하지만, 트윗 세트에서는 아직 벤치마크가 완전하지 않습니다 @alex_kirillov.

## 다양한 관점

### 지지/낙관적
- 전략적 승리로서의 오픈 웨이트 및 허용적 라이선스: 많은 이들이 Apache-2.0 출시를 미국/서구 오픈 에코시스템에 큰 활력을 불어넣는 것으로 보았습니다 @latkins, @saranormous, @brexton, @hyperindexed.
- 리더보드 경쟁보다 커스터마이징: 연구원들과 빌더들은 Inkling이 벤치마크 최고 성능을 목표로 하는 특정 솔루션이라기보다는 광범위하고 튜닝 가능한 파운데이션 모델이라는 명확한 프레이밍을 칭찬했습니다 @gneubig, @ben_burtenshaw, @thealexker.
- 강력한 출시 품질: 여러 사용자들은 투명성, 현실적인 어조, 포괄적인 기술 문서를 칭찬했습니다 @lvwerra, @saranormous, @rasbt.
- 아키텍처에 대한 관심: 비-RoPE 위치 선택과 스케일업된 짧은 컨볼루션 사용은 TML이 의미 있는 아키텍처 베팅을 할 의지가 있다는 증거로 긍정적인 관심을 끌었습니다 @stochasticchasm, @rasbt, @ChangJonathanC.

### 중립/분석적
- 강력하지만 전반적으로 최고는 아님: 가장 균형 잡힌 분석은 Inkling을 새로운 미국 오픈 웨이트 리더로 평가하지만, 일부 측면에서는 GLM/Kimi/DeepSeek 또는 최고 수준의 클로즈드 모델에 뒤처진다고 봅니다 @natolambert, @ArtificialAnlys, @stochasticchasm.
- 좋은 베이스 모델 가설: 여러 분석가들은 이번 출시를 시스템/비즈니스적 움직임으로 해석했습니다: 견고하고 효율적이며 후속 학습이 가능한 베이스 모델을 출시하고 Tinker와 다운스트림 RL/파인튜닝을 통해 차별화를 창출하는 것입니다 @ben_burtenshaw, @kimmonismus, @tinkerapi.

### 비판적/회의적
- 전반적으로 프론티어 모델은 아님: 비평가들은 여전히 최고 수준의 중국 오픈 웨이트 모델과 가장 강력한 클로즈드 모델에 명백히 뒤처진다고 주장했습니다 @scaling01, @JJitsev.
- 순수성 주장이 과장됨: 일부 반발은 독특하게 "순수"하거나 증류되지 않았다는 과장된 주장에 집중되었습니다. 스레드 세트에는 과대광고와 수정 사항이 모두 포함되어 있습니다 @jxmnop, @jxmnop, @andrew_n_carr, @JJitsev.
- 벤치마크의 중간 수준 성능에 대한 우려: 일부 독자들은 중간 수준의 벤치마크 프로필을 새로운 프론티어를 개척하기보다는 현재 중국 오픈 프론티어에 단순히 뒤처질 수 있다는 증거로 보았습니다 @scaling01.

## 맥락: 왜 이것이 중요한가
- TML의 첫 주요 공개 모델: 이는 전 OpenAI 리더 및 연구원들로 구성된 연구소에 대한 수개월간의 기대 끝에 Thinking Machines에서 출시된 첫 번째 진정한 외부 모델입니다. 따라서 오픈 웨이트 선택 자체가 주목할 만했습니다 @Hesamation, @TechCrunch.
- 중국의 모멘텀에 대한 미국의 오픈 웨이트 답변: 많은 반응들은 Inkling을 GLM, Kimi, DeepSeek, Qwen과 명시적으로 비교합니다. 이번 출시는 서구 오픈 웨이트 모델이 기능 및 출시 주기 면에서 중국 모델에 뒤처지고 있다는 우려 속에서 이루어졌습니다 @scaling01, @teortaxesTex, @sriramk.
- 오픈 베이스 + 후속 학습 스택 가설: TML의 메시지는 "유능한 오픈 기반을 출시한 다음, 커스터마이징/파인튜닝/RL 인프라를 통해 차별화한다"는 전략과 유사함을 강력히 시사합니다. 이는 Tinker 배포와 제어 가능한 추론, 간결한 출력, 적응에 중점을 둔 사용자 반응과 일치하며, 순수한 리더보드 우위를 추구하지 않습니다 @thinkymachines, @MichaelElabd, @ben_burtenshaw.
- 인퍼런스 에코시스템의 성숙도: 이번 출시는 또한 오픈 인퍼런스 스택이 얼마나 발전했는지 보여줍니다. 새로운 아키텍처 구성 요소와 여러 커널 수준 최적화를 갖춘 1조 파라미터급 멀티모달 MoE에 대한 출시 당일 지원은 1년 전에는 훨씬 덜 가능했을 것입니다 @vllm_project, @inferact, @LysandreJik.
- 대규모 아키텍처 실험: RoPE 대신 상대적 위치 바이어스와 대규모 짧은 컨볼루션 사용은 스케일링 및 후속 학습에서 견고함이 입증될 경우 미래 아키텍처 트렌드를 나타낼 수 있기 때문에 연구자들이 면밀히 주시하는 종류의 선택입니다 @stochasticchasm, @rasbt, @ChangJonathanC.
- 출시 스타일의 시그널: 여러 논평가들은 이례적으로 절제된 출시 언어, 전반적으로 가장 강력한 모델이 아니라는 명시적인 인정, 그리고 상세한 기술 노트를 칭찬했습니다. 전문가 청중에게는 이는 벤치마크 최고 성능을 목표로 하는 다른 출시작들에 비해 신뢰도를 높였습니다 @eliebakouch, @lvwerra, @thealexker.

## 7일 무료 체험으로 계속 읽어보세요
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-thinkys-inkling-975b-a41b&utm_source=paywall-free-trial&utm_medium=web&utm_content=207247810&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-thinkys-inkling-975b-a41b&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
