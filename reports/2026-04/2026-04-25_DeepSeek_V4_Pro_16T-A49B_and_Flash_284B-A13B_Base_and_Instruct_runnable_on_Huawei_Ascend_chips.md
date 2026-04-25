# DeepSeek V4 Pro (1.6T-A49B) and Flash (284B-A13B), Base and Instruct — runnable on Huawei Ascend chips

**원문 URL**: https://www.latent.space/p/ainews-deepseek-v4-pro-16t-a49b-and
**번역일**: 2026-04-25 06:21
**발행일**: 2026-04-25

---

[AINews: Weekday Roundups](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] DeepSeek V4 Pro (1.6T-A49B) 및 Flash (284B-A13B), Base 및 Instruct — Huawei Ascend 칩에서 실행 가능

### 돌아온 탕아 Tiger... 하지만 더 이상 벤치마크 리더는 아닙니다.
몇 달간의 지연과 많은 추측 끝에, DeepSeek은 마침내 오랫동안 기다려온 DSV4를 출시했습니다. 이는 DSV3 (2024년 12월) 및 DSR1 (2025년 1월) 이후 첫 번째 주요 버전 모델입니다. DSV4는 현재 오픈 모델 리더인 Kimi K2.6과 이틀 전 출시된 덜 알려진 Xiaomi Mimo 2.5와 함께 DeepSeek 제품군을 최신 라인업으로 끌어올렸습니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/a10f0270-c9c4-481b-962a-fcba50a2418b_1022x1104.png)
DSV4 제품군은 대략 Gemini 3.1, GPT 5.4, Opus 4.6 수준의 모델로, 최대 1.6T MoE를 사용하며 FP4로 32T 토큰에 대해 학습되었습니다. 1M 토큰 컨텍스트를 지원하며 (새로운 Compressed Sparse Attention (CSA) 및 Heavily Compressed Attention (HCA) 기술로 지원), 놀랍게도 Base 및 Instruct 버전을 모두 출시했습니다. 이는 향후 "DeepSeek R2"의 가능성을 위한 발판을 마련하는 것으로 보이며, 이 모델은 이미 추론 기능을 갖추고 있습니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/f028c03e-53a7-4615-af85-fc5e6e11dab0_1226x940.png)
기술 보고서는 일반적으로 58페이지에 달하는 방대한 내용으로, 1월에 발표된 Manifold Constrained Hyper-Connections (mHC) 논문에서 얻은 학습 및 인퍼런스 통찰력과 개선 사항, Moonshot의 Muon의 지속적인 사용, 그리고 DeepSeek 3.2-Exp의 이미 인상적인 Sparse Attention에 대한 CSA/HCA의 전반적인 놀라운 효율성 개선을 보여줍니다. 1M 토큰에서 DeepSeek-V3.2와 비교하여 FLOPs의 27%와 KV 캐시 메모리의 10%만 필요합니다.

![](https://substack-post-media.s3.amazonaws.com/public/images/f73baf75-34a0-46e8-8452-7cccd7481ba9_1156x730.png)
Huawei CANN 호환성 뒤에 있는 지정학적 배경은 DeepSeek이 수출 통제 대상인 NVIDIA/CUDA 칩에 대한 의존도를 줄이고 있다는 것입니다. Ascend는 여전히 H100s 공급량의 4분의 1에 불과하지만, 이는 중국의 완전한 독립을 위한 중요한 이정표입니다.
> 2026년 4월 23일~24일 AI 뉴스입니다. 저희는 12개의 서브레딧, 544개의 트위터를 확인했으며 추가 디스코드는 없습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션입니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
주요 소식: DeepSeek V4
DeepSeek은 V3 이후 첫 번째 주요 아키텍처 업데이트이자 첫 번째 명확한 2단계 라인업인 DeepSeek-V4 Pro와 DeepSeek-V4 Flash를 출시했습니다. 이 모델들은 1M 토큰 컨텍스트, 하이브리드 추론/비추론 모드, MIT 라이선스, 그리고 여러 연구자들이 올해 가장 중요하거나 잘 작성된 모델 논문 중 하나라고 평가할 만큼 상세한 기술 보고서를 특징으로 합니다. 전반적인 반응에서, V4가 오픈 웨이트 장문 컨텍스트 및 에이전틱 코딩 성능을 실질적으로 발전시켰지만, 전반적으로 최고 수준의 클로즈드 프론티어 모델들보다는 다소 뒤처진다는 사실적 합의가 있습니다. 독립적인 벤치마커들은 V4 Pro를 2위 오픈 웨이트 티어에 위치시키며, 벤치마크와 모드에 따라 Kimi K2.6 / GLM-5.1 / 강력한 Claude Sonnet급에서 Opus급에 가깝다고 평가합니다. 특히 장문 컨텍스트 및 에이전틱 성능이 강합니다. 이것이 "민주화"를 위한 진전인지, 아니면 소수의 오픈 랩만이 현실적으로 재현할 수 있을 정도로 복잡한 아키텍처인지에 대해서는 의견이 엇갈립니다. 주요 출처로는 @ArtificialAnlys, @scaling01, @nrehiew_, @ben_burtenshaw, @TheZachMueller, @ZhihuFrontier의 심층 분석 논평과 @vllm_project, @NVIDIAAI, @Togethercompute의 인프라/벤더 게시물이 있습니다.

## 핵심 사실 및 기술 세부 사항
논의 전반에 걸쳐 반복된 가장 구체적인 기술적 주장:
- 두 가지 모델
V4 Pro: 총 1.6T 파라미터 / 49B 활성
V4 Flash: 총 284B / 13B 활성
@ArtificialAnlys, @teortaxesTex, @baseten, @NVIDIAAI 보고
- 컨텍스트
@ArtificialAnlys에 따르면 V3.2의 128K에서 1M 토큰으로 증가했습니다.
여러 게시자들이 이를 주요 성과로 평가합니다: “견고한 초장문 컨텍스트” @teortaxesTex
- 학습 규모
32T–33T 토큰이 반복적으로 언급되었습니다.
@nrehiew_는 1.6T 파라미터에 걸쳐 32T 토큰, 즉 파라미터당 대략 20 토큰이라고 언급합니다.
@teortaxesTex는 33T를 인용합니다.
@nrehiew_는 사전 학습 컴퓨팅을 약 1e25 FLOPs로 추정합니다.
- 추론 / 모드
DeepSeek은 @Togethercompute에 따라 세 가지 추론 모드를 노출합니다.
하이브리드 “사고/비사고” 포지셔닝은 @ArtificialAnlys에 의해 언급되었습니다.
- 장문 컨텍스트 아키텍처
여러 스레드에서 새로운 하이브리드 어텐션 시스템을 요약합니다:
공유 KV 벡터
압축된 KV 스트림
압축된 토큰에 대한 희소 어텐션
인접 컨텍스트를 위한 로컬/슬라이딩 윈도우 어텐션
@ZhihuFrontier는 가장 간결한 공개 요약을 제공합니다:
공유 키-값 벡터를 통한 2배 KV 감소
c4a ≈ 4배 압축
c128a ≈ 128배 압축
압축된 토큰에 대한 top-k 희소 어텐션
128 토큰 슬라이딩 윈도우
1M 컨텍스트 KV 캐시 = 9.62 GiB/시퀀스 (bf16)
DeepSeek V3.2의 83.9 GiB보다 8.7배 작음
FP4 인덱스 캐시 + FP8 어텐션 캐시는 추가로 약 2배 감소를 제공합니다.
@ben_burtenshaw는 이를 “10배 더 작은 KV 캐시”로 요약합니다.
@TheZachMueller와 @TheZachMueller는 CSA + HCA 레이어 패턴을 설명하며, 교차 레이어와 V4 Flash가 일부 위치에서 HCA 대신 슬라이딩 윈도우 레이어를 사용한다고 언급합니다.
- 양자화 / 체크포인트 형식
@LambdaAPI: 체크포인트는 FP4 + FP8 혼합입니다.
MoE expert 가중치는 FP4
어텐션 / 정규화 / 라우터는 FP8
주장: 전체 모델이 단일 8×B200 노드에 적합합니다.
- 인퍼런스 하드웨어 / 서빙
@NVIDIAAI: Blackwell Ultra에서 V4 Pro는 에이전틱 워크플로우를 위해 150+ TPS/사용자 상호작용을 제공할 수 있습니다.
@NVIDIAAI: vLLM을 사용한 day-0 V4 Pro 성능 파레토를 발표했습니다.
@SemiAnalysis_: H200, MI355, B200, B300, GB200/300 전반에 걸친 day-0 지원 및 벤치마킹
@Prince_Canuma: 256GB Mac에서 DeepSeek4-Flash
@Prince_Canuma: MLX quants 발표
@simonw는 더 작은 RAM Mac의 실행 가능성에 대해 질문하며, 커뮤니티의 관심은 있지만 불완전한 지원 스토리를 암시합니다.
@QuixiAI는 많은 로컬 스택이 여전히 텐서 병렬을 지원하지 않는다는 점을 사용자들에게 상기시킵니다. 이는 V4급 모델이 인퍼런스 인프라에 강한 부담을 주기 때문에 중요합니다.
- 라이선스 / 가용성 / 가격
MIT 라이선스 (출처: @ArtificialAnlys)
1차 API 및 @Togethercompute, @baseten, @NousResearch, @Teknium을 통한 신속한 3차 가용성
V4 Pro 가격: 1M 입력/출력 토큰당 $1.74 / $3.48
V4 Flash 가격: $0.14 / $0.28
캐시 히트 가격도 @ArtificialAnlys에 의해 제공되었습니다.
@scaling01은 이 가격을 미래의 “Mythos급” 저렴한 코딩 모델의 엿보기로 봅니다.
@scaling01의 로이터 인용문: DeepSeek은 H2에 Huawei Ascend 950 슈퍼노드가 대규모로 배포되면 Pro 가격이 급격히 하락할 수 있다고 말했습니다.

## 독립적인 평가 및 V4의 위치
가장 유용한 독립 벤치마크 종합은 @ArtificialAnlys에서 나왔습니다:
- V4 Pro Max: Artificial Analysis Intelligence Index에서 52점
V3.2의 42점에서 10점 상승하여 Kimi K2.6 (54점)에 이어 2위 오픈 웨이트 추론 모델이 되었습니다.
- V4 Flash Max: 47점
강력한 중/고급 오픈 모델 수준으로 평가되며, “Claude Sonnet 4.6 최대 수준의 지능”입니다.
- GDPval-AA (에이전틱 실세계 작업):
V4 Pro: 1554점, 오픈 웨이트 모델 중 선두
Kimi K2.6 (1484점), GLM-5.1 (1535점), MiniMax-M2.7 (1514점)보다 앞섭니다.
- AA-Omniscience
V4 Pro: -10점, V3.2보다 11점 개선되었지만 여전히 94%의 환각률을 보입니다.
V4 Flash: 96% 환각률
- AA Index 실행 비용
V4 Pro: $1,071
V4 Flash: $113
- AA Index에서 사용된 출력 토큰
V4 Pro: 190M
V4 Flash: 240M
이는 중요한 주의사항입니다: 토큰당 가격이 저렴하다고 해서 모델이 엄청난 양의 토큰을 소비한다면 총 작업 비용이 저렴하다는 의미는 아닙니다.
추가 평가 관점:
- @arena:
데뷔 시 Text Arena 전체에서 2위 오픈 모델
카테고리 우승/순위:
#1 의료 및 건강
#15 창작 글쓰기
#18 다중 턴
사고 변형:
#8 수학
#9 생명/물리/사회 과학
- @arena는 Pro와 Flash의 트레이드오프를 강조합니다:
Pro는 약 30단계 더 높습니다.
비용은 12배 더 많이 듭니다.
Flash는 여전히 중국어, 의학, 수학 분야에서 경쟁력이 있습니다.
- @scaling01:
“~Opus 4.5 추정치는 적어도 SimpleBench에서는 현재 유효합니다.”
- @scaling01:
V4는 “확실히 GLM-5.1보다 낫지만 Opus 4.7, GPT-5.4 또는 Gemini 3.1 Pro에는 미치지 못합니다.”
- @scaling01은 6개월 미만의 격차를 확인할 수 있는 점수를 나열합니다:
ARC-AGI-1 ~75%
ARC-AGI-2 ~35%
GSO ~26%
METR 4.5–5시간
WeirdML ~63%
- @TheZachMueller:
자신의 평가에서 Flash@max ≈ Pro@high는 추론에서
Pro는 지식에 더 중점을 둡니다 (SimpleQA).
- @VictorTaelin:
벤치마크 버그를 수정하고 장시간 실행 모델을 더 오래 실행하도록 한 후, DeepSeek과 Kimi는 실질적으로 개선되었습니다.
- @mbusigin:
세부 사항 없는 단순한 부정적인 초기 인상
- @petergostev:
BullshitBench에서 능력보다는 거부/반발 행동에 관한 것으로, GPT-5.5는 저조한 성능을 보였습니다. 많은 독자들이 평가에 회의적인 환경에서 V4를 비교하기 때문에 여기에 포함되었습니다.

## 사실 대 의견

### 사실 / 비교적 잘 뒷받침되는 주장
- V4 Pro / Flash는 위에서 언급된 사양, MIT 라이선스, 1M 컨텍스트, 공개 기술 문서와 함께 출시되었습니다: @ArtificialAnlys, @TheZachMueller
- 이 아키텍처는 극적인 KV 캐시 감소를 특징으로 하는 새로운 장문 컨텍스트 어텐션 시스템을 도입합니다: @ZhihuFrontier, @ben_burtenshaw
- 독립적인 벤치마커들은 V4 Pro를 오픈 웨이트 모델 중 최상위권에 두지만, 전반적으로 최고의 독점 모델들보다는 아래에 위치시킵니다: @ArtificialAnlys, @arena, @scaling01
- DeepSeek V4는 일부 평가에서 토큰 사용량이 매우 많습니다: @ArtificialAnlys
- 체크포인트는 FP4/FP8 혼합 정밀도를 사용하며 8×B200 노드 하나에 적합합니다: @LambdaAPI
- vLLM 및 기타 제공업체를 통해 day 0에 신속한 생태계 지원이 이루어졌습니다: @vllm_project, @SemiAnalysis_

### 의견 / 해석
- @scaling01, @scaling01, @scaling01의 “V4는 프론티어 모델보다 약 4~5개월 뒤처져 있습니다”는 측정된 사실이 아닌 정보에 기반한 추정입니다.
- @teortaxesTex의 “오픈 모델 상위 3개” 대 “프론티어에 근접한 유일한 오픈 모델” 논쟁은 부분적으로 벤치마크 신뢰와 프레이밍에 관한 것입니다.
- @teortaxesTex의 “우리가 가진 가장 강력한 사전 학습 모델”은 직접적인 벤치마크 우위가 아닌 규모와 아키텍처에 기반한 의견입니다.
- @Dorialexander의 “올해 가장 중요한 AI 논문”은 합의가 아닌 열정입니다.
- @scaling01의 “이것이 연구가 나아가야 할 방향입니다”는 능력보다는 투명성/스타일에 대한 언급입니다.
- @teortaxesTex의 “정확히 민주화 기술은 아닙니다”는 강력한 아키텍처/정치적 해석입니다.

## 다른 의견과 주요 쟁점

### 1) V4는 프론티어에 근접한가, 아니면 명확히 뒤처져 있는가?
더 긍정적인 의견
- @scaling01: 대략 GPT-5.2 / Opus 4.5+ 티어에 위치시킵니다.
- @scaling01: SimpleBench는 약 Opus 4.5를 지지합니다.
- @teortaxesTex: 오픈 모델 중 가장 강력한 사전 학습 기반이며, 사람들이 사후 학습(post-training)이 할 수 있는 것을 과소평가하고 있다고 주장합니다.
더 회의적인 의견
- @scaling01: Opus 4.7 / GPT-5.4 / Gemini 3.1 Pro보다 아래입니다.
- @scaling01: 클로즈드 랩들이 더 큰 모델, 더 나은 과학/법률/의학 커버리지, GB200s를 통한 더 빠른 인퍼런스를 가지고 있기 때문에 격차가 다시 벌어질 수 있습니다.
- @mbusigin: 초기 인상이 “별로 좋지 않다”고 말합니다.
- @teortaxesTex: K2.6 및 GLM 5.1과 같은 정교한 모델들이 내재적 역량은 낮더라도 코딩에서 더 좋게 느껴질 수 있다고 말합니다.

### 2) V4의 진정한 기여는 모델 품질인가, 아니면 장문 컨텍스트 시스템 설계인가?
반응의 큰 분할점은 많은 기술 독자들이 장문 컨텍스트 아키텍처가 순수한 벤치마크 위치보다 더 중요하다고 생각한다는 것입니다.
- @teortaxesTex: “그들은 그들의 목표를 달성했습니다: 견고한 초장문 컨텍스트”
- @ben_burtenshaw: 장문 컨텍스트와 에이전틱 사후 학습(post-training)이 “만나는” 첫 번째 오픈 모델
- @scaling01: 다른 오픈 랩들이 이 아키텍처의 일부를 채택할 것으로 예상합니다.
- @Dorialexander: Huawei/주권 제약을 하드웨어 및 메모리/인터커넥트 설계를 재구성할 기회로 봅니다.
- @jukan05: 이 논문을 MoE/장문 컨텍스트 모델이 나아가는 방향과 NVIDIA의 하드웨어 로드맵이 이례적으로 잘 정렬되어 있다는 증거로 해석합니다.

### 3) V4는 “오픈 민주화”인가, 아니면 복제하기 너무 어려운가?
이것은 가장 첨예한 전략적 의견 불일치 중 하나였습니다.
- @teortaxesTex: V4는 아키텍처가 대부분의 랩에서 복제하기 너무 어렵기 때문에 “정확히 민주화 기술은 아닙니다”라고 말합니다.
- @teortaxesTex: DeepSeek조차도 리팩토링 없이 이 정확한 아키텍처를 다시 만들고 싶어 하지 않을 수 있다고 제안합니다.
- @stochasticchasm: 엄청난 하이퍼파라미터 복잡성이 daunting하다고 언급합니다.
- 이에 반해, @Prince_Canuma와 @Prince_Canuma는 생태계가 이미 Flash를 로컬 Apple Silicon 사용을 위해 압축하고 적용하고 있음을 보여주며, 학습 측면은 아니더라도 인퍼런스 측면에서 “민주화가 아니다”라는 주장을 완화합니다.

### 4) 사람들이 Flash를 과소평가하고 있는가?
여러 반응들은 Flash가 실제 채택에 있어 Pro보다 더 중요할 수 있음을 시사합니다.
- @arena: Flash는 가격/성능 프론티어를 변화시킵니다.
- @TheZachMueller: 추론 작업에서 Flash@max ≈ Pro@high
- @teortaxesTex: 벤치마크는 “푼돈으로 합법적인 1M 컨텍스트”를 과소평가할 수 있습니다.
- @Prince_Canuma: Flash는 256GB Mac에서 실행됩니다.
- @baseten과 @Togethercompute는 Flash의 경제성이 중요한 장문 문서 분석 및 에이전틱 사용 사례를 강조합니다.

## 중국, 칩, Huawei, 그리고 주권 컨텍스트
DeepSeek V4는 순수한 모델 출시로 논의되지 않았습니다. 이는 더 큰 미중 컴퓨팅 및 주권 논쟁의 증거로 다루어졌습니다.
- @scaling01: 중국 랩들은 모델이 더 나은 모델을 구축하는 데 도움이 된다는 점에서 이미 “도약” 단계에 있거나 근접해 있지만, 여전히 5개월 이상 뒤처져 있습니다.
- @scaling01: 칩 금지가 시간이 지남에 따라 광범위한 영역에서 격차를 벌릴 가능성이 있다고 생각합니다.
- @teortaxesTex, @teortaxesTex: Huawei를 단순하게 일축하는 것에 반박하며 Huawei에 대한 중국 내 다양한 정서를 언급합니다.
- @ogawa_tter: Ascend 950 / A3 클러스터 및 V4 배포 계획 분석을 지적합니다.
- @Dorialexander: Huawei를 둘러싼 주권 경쟁이 하드웨어 아키텍처를 재구성할 수 있다고 주장합니다.
- @scaling01: DeepSeek이 H2에 Ascend 950 슈퍼노드가 대규모로 배포되면 가격이 급격히 하락할 수 있다고 말한 것을 인용합니다.
- @jukan05: V4를 NVIDIA의 Blackwell/Rubin/HBM/인터커넥트 전략을 입증하는 것으로 해석합니다.
- @NVIDIAAI, @NVIDIAAI: 놀랄 것도 없이 Blackwell day-0 성능을 강조하지만, 이는 전략적 우월성에 대한 독립적인 증거라기보다는 벤더의 프레이밍입니다.
더 이념적인 측면도 있습니다:
- @teortaxesTex, @teortaxesTex, @teortaxesTex는 서구 담론이 종종 중국 랩들을 순전히 국가 대리인이나 디스틸레이션 샵으로 오해하지만, 실제로는 진지한 사명 지향적 행위자로 본다고 주장합니다. 이는 해석적인 부분이지만, 이번 출시가 왜 그렇게 감정적으로 격앙된 지정학적 반응을 불러일으켰는지 설명하는 데 도움이 됩니다.

## 디스틸레이션, 학습 데이터, 그리고 데이터 품질
반복되는 암묵적인 질문: V4는 주로 아키텍처 혁신을 반영하는가, 아니면 비평가들이 이를 “디스틸레이션”으로 일축할 수 있는가?
- @yacineMTB는 중국 디스틸레이션에 대한 일부 불만이 부분적으로 자신들이 성능에서 뒤처진다는 것을 발견한 사람들로부터 나올 수 있다고 추측합니다.
- @cloneofsimo: “매우 흥미롭네요... 그들이 Claude를 디스틸레이션했다는 점을 고려하면 🤔🤔”
- @kalomaze: DeepSeek이 DeepSeek 추론 흔적을 학습했다는 농담을 합니다.
- 더 실질적인 측면에서, @teortaxesTex는 DeepSeek의 글쓰기 품질, 특히 중국어의 경우, 데이터 청결도에 대한 오랜 집착을 반영한다고 말하며 @teortaxesTex, @teortaxesTex의 채용 공고를 인용합니다.
- @nrehiew_는 보고서가 표준 범주를 넘어선 사전 학습 데이터에 대한 자세한 내용이 여전히 부족하다고 언급합니다.
- 전반적으로, 이 트윗 세트의 사실적 공개 증거는 “DeepSeek이 강력한 데이터 작업을 통해 대규모로 학습한다”는 것을 지지하지만, 추측을 넘어선 외부 디스틸레이션의 정도에 대한 강력한 주장은 없습니다.

## 아키텍처 계보 및 선행 연구
여러 연구자들은 V4가 갑자기 나타난 것이 아니라고 지적했습니다.
- @jaseweston: DeepSeek이 2021년 ParlAI 접근 방식의 해시 라우팅을 사용한다고 말합니다.
- @suchenzang: 라우팅으로 인한 이상치(outliers)를 비판하며 해싱에 대한 비난을 가합니다.
- @teortaxesTex: Mixtral 스타일의 MoE가 합리적인 초기 해킹이었지만, DSMoE가 상황을 바꿨다고 주장합니다.
- @art_zucker는 MoE를 막다른 길로 광범위하게 공격합니다.
- @gabriberton은 MoE가 우아하지 않음에도 불구하고 입증 가능한 효과가 있다고 반박합니다.
- @stochasticchasm은 더욱 긍정적입니다: “MoE는 놀랍습니다”
이것이 중요한 이유는 V4가 단순히 더 강력한 체크포인트가 아니라, 오픈 장문 컨텍스트 MoE를 위한 가능한 새로운 설계 지점으로 읽혔기 때문입니다.

## 기술 보고서 자체가 중요했던 이유
모델뿐만 아니라 논문/보고서의 품질에도 놀라울 정도로 많은 칭찬이 쏟아졌습니다.
- @scaling01: “기술 논문은 매우 중요합니다”
- @Dorialexander: “올해 가장 중요한 AI 논문”
- @morqon: “내가 읽은 것 중 최고 중 하나”
- @scaling01: “이것이 연구가 나아가야 할 방향입니다”
- @TheZachMueller, @iamgrigorev, @nrehiew_: 모두 보고서를 소화하고 테스트하는 데 이례적으로 높은 노력을 기울였음을 시사합니다.
전문 독자들에게 이것은 중요합니다. 왜냐하면 많은 프론티어 모델 출시가 이제는 희소한 기술 공개와 함께 이루어지기 때문입니다. V4의 보고서는 진지한 오픈 출시가 어떤 모습이어야 하는지에 대한 기대를 재설정하는 것으로 보입니다.

## 실제적인 한계 및 주의사항
열정에도 불구하고, 몇 가지 주의사항이 반복적으로 언급됩니다:
- 집계된 능력에서 여전히 클로즈드 프론티어 모델에 뒤처집니다.
특히 @scaling01에 따르면 과학/법률/의학 및 광범위한 “일반 도메인”에서 그렇습니다.
- 추론 RL이 미숙할 수 있습니다.
@scaling01: V3.2 Speciale와 비교하여 추론 효율성은 크게 변하지 않았습니다.
- 서빙은 여전히 어렵습니다.
@scaling01: 많은 랩들이 20–30 tok/s의 속도와 제한된 동시성으로만 서빙하며, 평가 실행에는 하루가 걸릴 수 있습니다.
@ClementDelangue: HF에서 동시성 병목 현상을 인정합니다.
- 높은 토큰 사용량
@ArtificialAnlys의 주요 실용적 주의사항
- API 제어
@stochasticchasm: DeepSeek API가 샘플러 제어를 허용하지 않는 것으로 보인다고 언급합니다.
- 채택 가능성
@teortaxesTex: 많은 랩들이 깔끔하게 복사하기에는 너무 복잡합니다.

## 광범위한 시사점
세 가지 시사점이 두드러집니다.
1. 오픈 웨이트 장문 컨텍스트는 더 이상 단순한 마케팅이 아닙니다.
V4의 가장 강력한 기여는 구체적인 KV 캐시 엔지니어링과 오픈 인퍼런스 지원을 통해 1M 컨텍스트가 오픈 웨이트 모델에서 운영적으로 신뢰할 수 있음을 증명했다는 점일 수 있습니다. 이것이 여러 게시자들이 벤치마크 차이보다는 시스템 설계에 더 집중한 이유입니다: @ben_burtenshaw, @ZhihuFrontier, @scaling01.
2. 중국의 최고 랩들은 클로즈드 모델과의 격차를 완전히 좁히지 못하더라도 오픈 모델 분야에서는 여전히 경쟁력을 유지합니다.
@ArtificialAnlys, @arena, @scaling01의 벤치마크 결과는 Kimi, GLM, DeepSeek, 그리고 곧 MiMo와 같은 중국 랩들이 오픈 웨이트 최고 티어의 많은 부분을 지배하고 있음을 시사합니다.
3. “오픈”의 기준이 체크포인트 출시에서 풀스택 공동 설계로 높아지고 있습니다.
V4는 vLLM, Blackwell, MLX quants, Mac 실행 가능성, Ascend 클러스터, 캐시/메모리 아키텍처와 함께 즉시 논의되었습니다. 다시 말해, “모델”은 인퍼런스 기반과 점점 더 분리될 수 없게 되고 있습니다.

---
# 인프라, 인퍼런스, 그리고 로컬/오픈 생태계
- Hugging Face는 ML 작업을 위한 오픈소스 CLI “AI 인턴”인 ML Intern을 출시했습니다. 이는 논문 연구, 코드 작성, 실험 실행, HF 데이터셋/작업 사용, GitHub 검색, 최대 300단계 반복을 수행할 수 있습니다 (출처: @MillieMarconnni). 관련 의견: HF의 $9 Pro 티어는 @getpy에 따르면 이례적으로 강력한 가치를 제공합니다.
- Meta는 수십억 명의 사용자를 위한 Meta AI 및 에이전틱 시스템 확장을 위해 AWS Graviton 코어 수천만 개를 컴퓨팅 포트폴리오에 추가할 것이라고 밝혔습니다 (출처: @AIatMeta).
- 로컬/오픈 코딩 스택의 모멘텀은 강세를 유지했습니다:
@julien_c: MacBook Pro에서 llama.cpp를 통해 Qwen3.6-27B는 많은 코딩 작업에서 최신 Opus에 근접하게 느껴집니다.
@p0: Pi + Ollama + Gemma 4 + 병렬 웹 검색 MCP로 구축된 무료 CLI 에이전트
@Prince_Canuma: DeepSeek V4 quants 출시 예정
@QuixiAI: llama.cpp / Ollama / LM Studio는 텐서 병렬을 지원하지 않으므로, 진지한 다중 GPU 서빙 사용자들은 vLLM으로 이동해야 한다는 점을 상기시킵니다.
- Nous/Hermes는 활발하게 출시했습니다:
Hermes Agent v0.11.0은 재작성된 React TUI, 대시보드 플러그인, 테마, 더 많은 인퍼런스 제공업체, 이미지 백엔드, QQBot 지원을 도입했습니다 (출처: @WesRoth).
Hermes는 @mr_r0b0t, @Teknium을 통해 DeepSeek V4와 GPT-5.5 모두에 대해 폭넓은 찬사와 신속한 지원을 받았습니다.
@JulianGoldieSEO와 @LoicBerthelot는 학습 루프, 메모리, 모델 지원, 배포 유연성, 보안 측면에서 Hermes를 OpenClaw와 비교하여 호의적으로 평가했습니다.
bubblewrap + cgroups v2를 사용하는 Deep Agents용 네이티브 Linux 샌드박스 백엔드가 @nu_b_kh에 의해 출시되었습니다.
연구 논문 및 벤치마크
- 온-폴리시 디스틸레이션 토큰 선택:
@TheTuringPost는 일부 토큰만이 대부분의 학습 신호를 전달한다는 논문을 강조합니다. 약 50%의 토큰을 사용하면 전체 학습과 일치하거나 능가할 수 있으며 메모리를 약 47% 절감할 수 있고, 심지어 10% 미만의 확신 없는(confident-wrong) 토큰에 집중해도 거의 전체 학습과 일치합니다.
- Google Research는 여러 ICLR 데모를 발표했습니다:
MesaNet, 고정 메모리 하에서 인컨텍스트 학습에 최적화된 트랜스포머 대체 / 선형 시퀀스 레이어 (출처: @GoogleResearch)
로보틱스/3D 추론 및 효율적인 트랜스포머 작업 (출처: @GoogleResearch)
“추론이 정직함으로 이어질 수 있다” 데모 (출처: @GoogleResearch)
- MIT Hyperloop Transformers는 루프형 및 일반 트랜스포머 블록을 혼합하여 약 50% 적은 파라미터를 사용하면서 240M / 1B / 2B에서 일반 트랜스포머를 능가합니다 (출처: @TheTuringPost).
- “Learning mechanics”는 딥러닝 역학 이론을 종합하려고 시도합니다 (출처: @learning_mech).
- 도구/에이전트 시스템 논문:
Tool Attention Is All You Need는 동적 게이팅 및 지연 스키마 로딩을 통해 95%의 도구 토큰 감소(47.3k → 2.4k/턴)를 주장합니다 (출처: @omarsar0).
장기 구조화된 메모리를 위한 StructMem이 @dair_ai에 의해 강조되었습니다.
HorizonBench는 변화하는 사용자 선호도를 가진 장기 개인화를 목표로 합니다 (출처: @StellaLisy).
- 소프트웨어 엔지니어링을 위한 명확화 질문:
@gneubig는 명확화 질문을 하도록 특별히 학습된 모델에 대한 작업을 공유했으며, 더 적은 질문으로 결과를 개선했습니다.
GPT-5.5 출시 및 코딩 에이전트
- OpenAI는 1M 컨텍스트 윈도우를 갖춘 GPT-5.5 및 GPT-5.5 Pro를 API 및 생태계 제품에 출시했습니다 (출처: @OpenAI, @OpenAIDevs).
- Cursor, GitHub Copilot, Codex/OpenAI API, OpenRouter, Perplexity, Devin, Droid, Fleet, Deep Agents 전반에 걸쳐 즉시 배포되었습니다:
@cursor_ai: GPT-5.5는 CursorBench에서 72.8%로 1위입니다.
@cline: Terminal-Bench에서 82.7%로 1위입니다.
@OpenAIDevs: Perplexity Computer는 복잡한 작업에서 56% 더 적은 토큰을 사용했습니다.
@scaling01: GPT-5.5 medium은 LisanBench에서 GPT-5.4 medium보다 45.6% 적은 토큰으로 더 높은 점수를 기록하며 가장 강력한 비사고 모델이 되었습니다.
- 사용자 피드백은 일부 평가에 대한 엇갈린 감정에도 불구하고 더 나은 코딩 품질과 토큰 효율성에 집중되었습니다:
@almmaasoglu: LLM에서 읽은 최고의 코드; 덜 장황하고, 덜 방어적입니다.
@KentonVarda: 6년 전 댓글에서 깊은 Cap’n Proto RPC 코너 케이스를 발견했습니다.
@willdepue: 평가에는 실망했지만, 복잡한 기술 프로젝트에서 Codex에 감명받았습니다.
@omarsar0: 더 나은 “노력 보정(effort calibration)” 덕분에 Claude Code에서 Codex/GPT-5.5로 원활하게 전환했습니다.
- Cursor는 또한 /multitask 비동기 서브에이전트 및 다중 루트 워크스페이스를 출시했습니다 (출처: @cursor_ai).
- 작은 품질 격차보다는 한계와 경제성에 대한 시장의 강조가 커지고 있습니다:
@nrehiew_는 이제 작은 프론티어 모델 차이보다 사용량 제한이 더 중요하다고 주장합니다.
@HamelHusain은 Codex의 구독 구조 때문에 사용하지 않기 어렵다고 말합니다.
산업 동향, 자금 조달 및 정책
- Google은 Anthropic에 최대 $40B를 투자할 계획이라고 보도되었습니다 (출처: @FT, @zerohedge). 반응은 Anthropic의 컴퓨팅 약정이 이제 얼마나 커질 수 있는지에 집중되었습니다.
- Cohere와 Aleph Alpha는 캐나다/독일 주권 AI 파트너십을 발표했으며, @cohere, @aidangomez, @nickfrosst에 의해 엔터프라이즈급 및 개인 정보 보호/보안에 중점을 둔 것으로 평가되었습니다.
- ComfyUI는 $500M의 가치로 $30M를 유치했으며, 핵심/오픈-로컬 포지셔닝을 유지했습니다 (출처: @yoland_yan).
- Mechanize는 $500M의 투자 후 가치로 $9.1M를 유치했다고 발표했습니다 (출처: @MechanizeWork).
- Arcee AI는 Cody Blakeney를 연구 책임자로 고용했으며, 오픈 웨이트 미국 프론티어 모델을 강조했습니다 (출처: @code_star).
- 안전성 / 거버넌스:
OpenAI는 GPT-5.5에 대한 Bio Bug Bounty를 발표했습니다 (출처: @OpenAINewsroom).
Anthropic은 직원들을 대신하여 Claude가 협상하는 마켓플레이스인 Project Deal을 출시했으며, 모델 품질 비대칭 및 정책 과제를 강조했습니다 (출처: @AnthropicAI).
크리에이티브 AI 및 멀티모달
- GPT Image 2 + Seedance 2 워크플로우는 계속해서 주목을 받았습니다:
@_OAK200과 @awesome_visuals는 고화질 이미지→비디오 파이프라인을 선보였습니다.
@BoyuanChen0은 2K/4K 이미지가 이미 실험용 API를 통해 제공되며 활발한 수정 작업이 진행 중이라고 말했습니다.
- Kling은 네이티브 4K 출력과 $25k 단편 영화 콘테스트를 발표했습니다 (출처: @Kling_ai).
- 일부 평가적 뉘앙스:
@goodside는 GPT Images 2.0이 유효해 보이는 루빅스 큐브 상태를 렌더링할 수 있었는데, 이는 놀랍도록 어려운 일이라고 언급했습니다.
@venturetwins는 최근 이미지/비디오의 발전이 개인화된 게임과 같은 콘텐츠 생성으로 나아가는 중요한 단계라고 평가했습니다.

---

# AI 레딧 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. Deepseek V4 and Related Releases
- Deepseek V4 AGI confirmed (Activity: 1138): 해당 이미지는 밈이며 기술적인 내용을 포함하고 있지 않습니다. ‘Deepseek V4 AGI confirmed’라는 제목은 AI 모델에 대한 유머러스하거나 과장된 주장으로, 인공 일반 지능(AGI)의 발전을 언급하는 것일 수 있습니다. 댓글들은 검열되지 않은 데이터셋과 군사적 적용을 언급하며 풍자적인 어조를 더욱 암시하는데, 이는 진지한 주장이 아닐 가능성이 높습니다. 댓글들은 검열되지 않은 데이터셋과 군사적 적용을 언급하며 AI 역량에 대한 풍자적인 시각을 반영하고 있으며, 진지한 기술적 논의보다는 회의론이나 유머를 나타냅니다. UserXtheUnknown은 Deepseek V4의 테스트 시나리오를 논의하며, 문제가 발생했을 때 과도하게 생각하는 경향을 강조합니다. 이 모델은 ‘칼 하나만 사용하기’와 같은 제약 조건을 선택 사항이 아닌 필수 사항으로 해석하여 문제 해결 방식에 영향을 미칩니다. 이는 작업 제약 조건에 대한 미묘한 이해를 반영하지만, 암묵적인 지시를 처리하는 데 있어 개선될 수 있는 잠재적 영역도 나타냅니다.
- Deepseek V4 Flash and Non-Flash Out on HuggingFace (Activity: 1393): DeepSeek V4가 HuggingFace에 출시되었습니다. 이 모델은 1.6T 파라미터(이 중 49B가 활성화됨)를 가진 DeepSeek-V4-Pro와 284B 파라미터(이 중 13B가 활성화됨)를 가진 DeepSeek-V4-Flash 두 가지 모델을 특징으로 합니다. 두 모델 모두 100만 토큰의 컨텍스트 길이를 지원하며, 이는 광범위한 시퀀스를 처리하는 데 중요합니다. 이 모델들은 MIT 라이선스 하에 출시되어 광범위한 사용 및 수정이 가능합니다. 주목할 만한 댓글은 이러한 대규모 모델을 다룰 때 하드웨어 제약, 특히 RAM의 어려움을 강조합니다. 다른 댓글은 모델 크기를 보다 효과적으로 관리하기 위해 0.01bit 퀀티제이션(quantization)의 잠재적 이점을 제안합니다. DeepSeek-V4 모델은 방대한 파라미터 크기로 주목받고 있으며, Pro 버전은 1.6조 파라미터(490억 활성화), Flash 버전은 2,840억 파라미터(130억 활성화)를 가집니다. 두 모델 모두 100만 토큰의 광범위한 컨텍스트 길이를 지원하며, 이는 대규모 데이터 입력 및 복잡한 작업을 처리하는 데 중요합니다. 한 사용자는 DeepSeek-V4 모델의 0.01비트 퀀티제이션에 관심을 표명했는데, 이는 성능을 유지하면서 모델 크기와 계산 요구 사항을 줄이는 데 중점을 두고 있음을 시사합니다. 퀀티제이션은 제한된 리소스를 가진 하드웨어에 모델을 배포하기 위해 모델을 최적화하는 일반적인 기술입니다. MIT 라이선스 언급은 DeepSeek-V4가 오픈소스이며, 커뮤니티에 의한 광범위한 사용 및 수정을 허용함을 나타냅니다. 이러한 라이선스 선택은 개발자들이 모델을 자신들의 프로젝트에 자유롭게 통합하고 적용할 수 있으므로 협업과 혁신을 촉진할 수 있습니다.
- Buried lede: Deepseek v4 Flash is incredibly inexpensive from the official API for its weight category (Activity: 404): 해당 이미지는 “deepseek-v4-flash”와 “deepseek-v4-pro” 두 모델 간의 비교를 제공하며, “deepseek-v4-flash” 모델이 입력 및 출력 토큰 비용 측면에서 훨씬 더 저렴하다는 점을 강조합니다. 저렴함에도 불구하고, 이 모델은 JSON 출력, 툴 콜, 그리고 비사고 모드와 사고 모드 모두에서 챗 프리픽스 완성(chat prefix completion)과 같은 고급 기능을 지원합니다. 이미지를 둘러싼 논의는 “deepseek-v4-flash”가 저렴하다고 홍보되지만, 일부 사용자들은 파라미터 스케일링을 고려할 때 이전 버전에 비해 실제로는 과도하게 비싸다고 주장하며, “V3.2” 모델이 파라미터당 더 저렴하다고 말합니다. 댓글 작성자들은 GPU 부족이 현재 가격에 미치는 영향을 논의하며, GPU 생산이 증가함에 따라 가격이 하락할 수 있다고 제안합니다. 또한 가격 전략에 대한 논쟁도 있으며, 일부 사용자들은 새 모델이 이전 버전에 비해 파라미터당 더 비싸다고 지적합니다. DistanceSolar1449는 DeepSeek V3.2와 V4 Flash 간의 가격 비교를 강조하며, V3.2는 671B에서 입력/출력에 $0.26/$0.38로 가격이 책정되었고, V4 Flash는 284B에서 $0.14/$0.28이라고 언급합니다. 이는 가격이 파라미터에 비례하여 선형적으로 스케일링된다면 V4 Flash가 실제로는 더 비싸다는 것을 시사하며, 비용 효율성이라는 개념에 이의를 제기합니다. jwpbe는 DeepSeek V4 Flash의 API 비용에 대한 비교 분석을 제공하며, 입력 14센트/출력 28센트의 가격으로 Minimax 2.7과 같은 경쟁사(3배 비쌈) 및 Qwen의 동급 모델(더 비쌈)보다 훨씬 저렴하다고 말합니다. 그들은 또한 Trinity Thinking Large가 두 배 더 비싸다고 언급하며, V4 Flash가 시장에서 경쟁력 있는 가격 우위를 제공함을 나타냅니다. Worried-Squirrel2023은 Huawei의 실리콘 개발이 가지는 전략적 함의를 논의하며, DeepSeek의 가격 전략이 NVIDIA 마진을 Ascend 공급과 교환하는 것을 포함한다고 제안합니다. 그들은 950 슈퍼노드가 스케일링되면 DeepSeek이 Huawei의 발전을 활용하여 비용을 최적화함으로써 오픈 웨이트(open weights) 계층의 경쟁사들을 잠재적으로 능가할 수 있다고 예측합니다.
- Deepseek has released DeepEP V2 and TileKernels. (Activity: 396): Deepseek이 AI 모델 최적화 및 병렬화에 있어 중요한 발전인 DeepEP V2와 TileKernels를 출시했습니다. DeepEP V2는 모델 효율성과 정확성 향상에 중점을 두는 반면, TileKernels는 계산 용량을 두 배로 늘리면 처리 속도도 두 배가 되는 선형적으로 스케일링되는 새로운 병렬화 기술을 도입했습니다. 이 릴리스는 오픈소스이며, AI 연구의 투명성과 협업을 촉진합니다. 더 자세한 내용은 DeepEP V2 풀 리퀘스트와 TileKernels 레포지토리에서 확인할 수 있습니다. 한 댓글 작성자는 Deepseek이 연구를 발전시키고 결과를 공개적으로 공유함으로써 OpenAI가 수행할 것으로 기대되었던 역할을 수행하고 있으며, 이는 독점 기술에도 불구하고 선의를 구축한다고 강조합니다. 다른 댓글 작성자는 병렬화 기술이 실제로 선형적으로 스케일링되는지 의문을 제기하며, 사실이라면 상당한 기술적 돌파구가 될 것이라고 제안합니다. DeepEP V2와 TileKernels by DeepSeek은 병렬화 기술의 잠재적 발전으로 주목받고 있습니다. 한 사용자는 이러한 기술이 선형 스케일링을 달성할 수 있으며, 이는 계산 용량을 두 배로 늘리면 처리 속도도 직접적으로 두 배가 될 수 있음을 의미한다고 추측합니다. 이는 모델 학습(training) 및 인퍼런스(inference)에서 상당한 효율성 개선을 나타낼 수 있습니다. DeepSeek의 하드웨어 사용, 특히 SM100 및 Blackwell GPU에 대한 추측이 있습니다. 한 댓글 작성자는 DeepSeek이 Vast.ai에서 B200 유닛을 임대하여 Blackwell GPU를 학습(training)에 사용하고 있을 수 있다고 제안합니다. 이러한 하드웨어 선택은 모델의 성능과 역량에 영향을 미칠 수 있습니다. DeepSeek의 다음 모델(아마도 v4로 명명될)의 잠재적 혁신이 강조됩니다. Engram 및 mHC 기술의 통합에 초점이 맞춰져 있으며, 이는 모델 성능에 중요한 역할을 할 것으로 예상됩니다. 이러한 혁신의 성공은 DeepSeek이 개발한 새로운 데이터셋에 달려 있을 것입니다.

### 2. Qwen 3.6 Model Performance and Benchmarks
- This is where we are right now, LocalLLaMA (Activity: 1755): 해당 이미지는 MacBook Pro에서 Llama.cpp를 통해 Qwen3.6 27B 모델을 실행하는 모습을 보여주며, 비행기 모드에서도 복잡한 AI 모델을 로컬에서 실행할 수 있는 역량을 강조합니다. 이는 클라우드 서비스와 독립적으로 작동함으로써 로컬 AI 모델이 효율성, 보안, 프라이버시 및 주권을 향상시킬 잠재력을 강조합니다. 이 게시물은 강력한 AI 모델을 개인 장치에서 접근 가능하게 만드는 기술적 발전을 강조하며, 프라이버시와 제어를 위한 로컬 실행의 중요성을 역설합니다. 댓글 작성자들은 Qwen3.6-27B 모델의 역량에 대한 과장된 주장에 회의적인 시각을 표명하며, 크기에 비해 인상적이지만 Sonnet 또는 Opus와 같은 더 발전된 모델의 성능에는 미치지 못한다고 제안합니다. 과장된 주장이 사용자 실망과 더 넓은 LLM 커뮤니티에 대한 반발로 이어질 수 있다는 우려가 있습니다. ttkciar는 Qwen3.6-27B 모델에 대한 사용자 실망 가능성을 강조하며, 크기에 비해 인상적이고 에이전틱(agentic) 코드 생성에 적합하지만 Sonnet 또는 Opus와 같은 더 발전된 모델의 역량에는 미치지 못한다고 지적합니다. 능력에 대한 과도한 홍보가 주장을 하는 개인뿐만 아니라 더 넓은 LLM 커뮤니티에 대한 반발로 이어질 수 있다는 우려가 있습니다. sooki10은 이 모델이 로컬 코딩 작업에 인상적이지만, Opus와 같은 더 발전된 모델과 비교하는 것은 오해의 소지가 있으며 제기된 주장의 신뢰성을 훼손할 수 있다는 점에 동의합니다. 이는 사용자 기대를 효과적으로 관리하기 위해 모델 역량에 대한 더 정확한 벤치마킹(benchmarking) 및 소통의 필요성을 시사합니다. Melodic_Reality_646은 리소스의 불균형을 지적하며, 고성능 128GB RAM m5max 시스템 사용을 더 접근하기 쉬운 설정과 비교합니다. 이는 모델 성능을 평가할 때 하드웨어 제약 조건을 고려하는 것의 중요성을 강조합니다. 모든 사용자가 이러한 강력한 시스템에 접근할 수 있는 것은 아니며, 이는 모델 역량에 대한 인식을 왜곡할 수 있기 때문입니다.
- DS4-Flash vs Qwen3.6 (Activity: 470): 해당 이미지는 DS4-Flash Max와 Qwen3.6 모델, 특히 35B-A3B 및 27B 버전 간의 벤치마크(benchmark) 비교를 제시합니다. 차트는 DS4-Flash Max가 일반적으로 다양한 카테고리에서 Qwen 모델을 능가하며, 특히 ‘LiveCodeBench’ 및 ‘HLE’ 벤치마크에서 뛰어난 성능을 보인다는 점을 강조합니다. 이는 DS4-Flash Max가 코딩 및 추론(reasoning) 작업에서 우수한 역량을 가질 수 있음을 시사합니다. 댓글의 논의는 Qwen3.6의 122B 버전과 같은 더 큰 모델의 잠재력을 암시하며, ‘omniscense’와 같은 다른 벤치마크에서 성능에 영향을 미칠 수 있는 1M 토큰 컨텍스트(context) 기능의 중요성을 강조합니다. 댓글 작성자들은 DS4-Flash Max의 더 큰 크기에도 불구하고 성능이 Qwen3.6보다 약간만 더 좋다는 점을 지적하며, 효율성과 스케일(scale) 간의 질문을 제기합니다. 1M 토큰 컨텍스트는 향후 벤치마크 결과에 영향을 미칠 수 있는 중요한 기능으로 강조됩니다. Rascazzione은 Qwen 3.6의 컨텍스트 길이(context length)가 크게 증가했음을 강조하며, 100만 토큰 컨텍스트를 처리할 수 있는 능력을 언급합니다. 이는 이전 모델들에 비해 상당한 개선이며, 문서 요약이나 복잡한 대화 시스템과 같이 광범위한 컨텍스트 처리가 필요한 작업에 중요한 영향을 미칠 수 있습니다. LinkSea8324는 모델 간의 크기 차이를 지적하며, DS4-Flash는 2,840억 파라미터인 반면 Qwen 3.6은 270억 파라미터라고 언급합니다. 이는 모델 크기와 역량 간의 효율성 및 성능 트레이드오프, 특히 계산 리소스 및 인퍼런스(inference) 속도 측면에서 의문을 제기합니다. madsheepPL은 벤치마크 개선의 비선형적 특성을 논의하며, 모델이 벤치마크에서 약간만 더 좋게 보이더라도 실제 적용에서는 더 큰 의미를 가질 수 있다고 제안합니다. 그들은 점수 개선이 직접적으로 비례하지 않으며 실제 애플리케이션에 다양한 영향을 미칠 수 있음을 강조합니다.
- Qwen 3.6 27B Makes Huge Gains in Agency on Artificial Analysis - Ties with Sonnet 4.6 (Activity: 964): Qwen 3.6 27B는 Artificial Analysis의 에이전틱(Agentic) 인덱스에서 Sonnet 4.6과 동등한 수준을 달성했으며, Gemini 3.1 Pro Preview, GPT 5.2 및 5.3, MiniMax 2.7과 같은 모델들을 능가했습니다. 이 모델은 모든 인덱스에서 개선을 보였지만, 코딩 인덱스에서의 성과는 Terminal Bench Hard 및 SciCode와 같이 비전통적으로 간주되는 벤치마크(benchmark)에 의존하기 때문에 덜 두드러집니다. 학습(training)의 초점은 OpenClaw/Hermes를 위한 에이전틱 애플리케이션에 있는 것으로 보이며, 이는 소규모 모델이 프론티어(frontier) 역량에 접근할 잠재력을 강조합니다. 다가오는 Qwen 3.6 122B 모델에 대한 기대가 커지고 있습니다. 댓글 작성자들은 Qwen 3.6 27B와 같은 소규모 모델의 잠재력에 대한 흥분을 표현하며, 상당한 개선과 향후 버전의 가능성을 언급합니다. 그러나 이러한 성과의 정도에 대한 회의론도 있으며, 일부 개선은 모델의 본질적인 역량보다는 ‘벤치맥싱(benchmaxxing)’ 때문일 수 있다고 제안합니다. Iory1998은 Qwen 3.6 27B 모델의 인상적인 성능을 강조하며, 전년도 670B 모델을 능가한다고 언급합니다. 그들은 RTX 3090 및 RTX 5070ti에서 FP16 KV 캐시(KV cache)와 함께 Q8 버전을 170K로 실행하며 40GB VRAM을 활용했다고 언급하는데, 이는 모델의 효율성과 성능을 강조합니다. AngeloKappos는 벤치마크 격차가 좁혀지고 있음을 논의하며, M2 칩에서 Qwen3-30b-a3b 모델을 실행한 경험을 공유합니다. 그들은 이 모델이 다단계 툴 콜(tool calls)을 효과적으로 처리할 수 있는 능력을 지적하며, 27B 덴스(dense) 모델이 이 정도로 잘 수행한다면, 다가오는 122B 모델은 잠재적 성능으로 인해 API 제공업체에 어려움을 줄 수 있다고 제안합니다. Velocita84는 Qwen 3.6 27B 모델의 보고된 성능 향상에 잠재적인 “벤치맥싱”이 있을 수 있다는 점을 제기하며, 일부 개선이 모델의 본질적인 역량보다는 최적화된 벤치마킹(benchmarking)에 기인할 수 있음을 암시합니다. 이는 모델 성능 주장을 평가할 때 정밀 조사가 필요함을 시사합니다.
- Compared QWEN 3.6 35B with QWEN 3.6 27B for coding primitives (Activity: 491): 이 게시물은 MacBook Pro M5 MAX 64GB RAM 시스템에서 QWEN 3.6 모델의 두 가지 버전, 즉 35B 및 27B 파라미터 버전을 비교합니다. 35B 모델은 72 TPS(초당 토큰)를 달성하는 반면, 27B 모델은 18 TPS를 달성합니다. 더 느린 속도에도 불구하고, 27B 모델은 코딩 작업에서 더 정확하고 올바른 결과를 생성하는 반면, 35B 모델은 더 빠르지만 정확도가 떨어집니다. 이 테스트는 외부 라이브러리 없이 패럴랙스(parallax) 효과가 있는 움직이는 자동차를 시뮬레이션하기 위해 단일 HTML 파일을 생성하는 것을 포함했습니다. 모델은 Atomic.Chat을 사용하여 호스팅되었으며, 소스 코드는 GitHub에서 확인할 수 있습니다. 한 댓글은 opencode를 사용하여 Qwen 3.6 27B FP8 모델의 출력을 강조하며, 약 52초가 소요되었다고 언급합니다. 다른 댓글은 Qwen 3.5 27B Q3 모델과의 시각적 비교를 제공하며, 출력 품질의 차이를 시사합니다. 사용자 ‘sacrelege’는 FP8 정밀도를 사용하는 Qwen 3.6 27B 모델의 성능 결과를 공유하며, ‘opencode’로 작업을 완료하는 데 약 52초가 걸렸다고 언급했습니다. 이는 정밀도 조정을 통해 모델 성능을 최적화하는 데 중점을 두고 있음을 시사하며, 이는 계산 효율성과 속도에 상당한 영향을 미칠 수 있습니다. 사용자 ‘nikhilprasanth’는 Qwen 3.5 27B Q3 모델에 대한 시각적 비교를 제공하며, Qwen 모델의 다양한 버전 및 퀀티제이션(quantization) 수준을 비교하는 데 잠재적인 관심이 있음을 나타냈습니다. 이는 다양한 모델 구성이 성능과 출력 품질에 어떻게 영향을 미칠 수 있는지 이해하는 것의 중요성을 강조합니다. ‘Technical-Earth-3254’는 테스트에 사용된 퀀티제이션 방법에 대해 문의했는데, 이는 모델 크기, 속도 및 정확도 간의 트레이드오프를 이해하는 데 중요합니다. 퀀티제이션은 Qwen과 같은 대규모 모델의 효율성에 큰 영향을 미칠 수 있으며, 특히 리소스가 제한된 환경에서 더욱 그렇습니다.
- Qwen 3.6 27B is a BEAST (Activity: 1239): 이 게시물은 RTX 5090 GPU와 24GB VRAM을 갖춘 고성능 노트북에서 Qwen 3.6 27B 모델의 성능을 논의하며, pyspark/python 및 데이터 변환 디버깅 작업에 대한 효과를 강조합니다. 사용자는 q4_0에서 q4_k_m과 함께 llama.cpp를 사용하고 있으며, 200k q8_0에서 IQ4_XS를 통한 추가 최적화를 탐색하고 있습니다. 사용자는 아직 스페큘레이티브 디코딩(speculative decoding)을 구현하지 않았습니다. 설정에는 64GB DDR5 RAM을 갖춘 ASUS ROG Strix SCAR 18이 포함됩니다. 댓글들은 코딩을 위해 q4로 KV 캐시(KV cache)를 사용하는 것을 피하고, 130k 컨텍스트(context)를 위해 q8을 권장합니다. 다른 댓글은 z-lab의 다가오는 릴리스와 2배 디코드 속도 증가를 약속하는 특정 GitHub 풀 리퀘스트(pull request)를 통해 성능 개선을 예상합니다. 또한 16GB VRAM 및 32GB DDR5 RAM을 갖춘 시스템에서 오프로딩(offloading) 시 모델 성능에 대한 궁금증도 있습니다. sagiroth는 코딩 작업에 Qwen 3.6 27B를 사용할 때의 기술적 고려 사항을 강조하며, 제한 사항으로 인해 q4로 KV 캐시를 사용하는 것을 피하고, 대신 q8을 사용하여 130k 컨텍스트 윈도우(context window)를 달성할 것을 제안합니다. 이는 대규모 컨텍스트 작업의 성능을 크게 향상시킬 수 있습니다. inkberk는 llama.cpp 레포지토리의 풀 리퀘스트 #22105를 참조하며, 디코딩 속도의 다가오는 개선을 지적합니다. 이 업데이트는 z-lab의 ‘dflash drafter’의 예상 출시와 함께 디코드 속도를 잠재적으로 2배 증가시킬 것을 약속하며, 이는 효율성 측면에서 사용자에게 큰 이점을 줄 수 있습니다. Johnny_Rell은 16GB VRAM 및 32GB DDR5를 갖춘 시스템에서 Qwen 3.6 27B의 성능, 특히 오프로딩의 효과에 대해 문의합니다. 이는 모델의 요구 사항을 처리하기 위한 리소스 할당 최적화에 중점을 두고 있음을 시사하며, 이는 소비자용 하드웨어에서 대규모 모델을 효율적으로 실행하는 데 중요합니다.

## 7일 무료 체험으로 계속 읽어보세요
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-deepseek-v4-pro-16t-a49b-and&utm_source=paywall-free-trial&utm_medium=web&utm_content=195414627&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-deepseek-v4-pro-16t-a49b-and&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
