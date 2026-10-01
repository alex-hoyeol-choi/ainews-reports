# Gemini 4 Argon: GDM’s answer to Astra/Fable, with 1M output

**원문 URL**: https://www.latent.space/p/ainews-gemini-4-argon-gdms-answer
**번역일**: 2026-10-01 12:29
**발행일**: 2026-10-01

---

[AINews: 주중 요약](https://www.latent.space/s/ainews/?utm_source=substack&utm_medium=menu)
# [AINews] Gemini 4 Argon: 1M 출력으로 Astra/Fable에 대한 GDM의 답변

### ... 하지만 "Fairwind Program의 정부 사용자 및 신뢰할 수 있는 사이버 방어자"가 아니라면 아직 사용해 볼 수 없습니다
Oct 01, 2026공유GDM은 지난 2월 Flash보다 큰 모델(3.1 Pro)을 출시했으며, 연이은 점진적인 3.x Flash 버전들과 지난달의 대규모 GDM 경영진 개편 이후, GDM에게 가장 큰 질문은 그동안 Fable 및 Astra 클래스 모델을 출시한 경쟁사들을 언제 따라잡을 것인가였습니다.
음, Argon이 출시되었습니다. 매우 훌륭한 벤치마크 결과(19개 신뢰할 수 있는 벤치마크 중 13개에서 SOTA)를 보여주지만… 제한된 사이버 보안 프리뷰에서만 접근 가능하며, "가능한 한 빨리" 접근을 약속했습니다:

![X avatar for @GoogleDeepMind](https://pbs.substack.com/profile_images/1695024885070737408/-M-HSH5P.jpg)
저희는 업계 최초로 출력 토큰을 최대 1M까지 늘리는 실험적인 Long Decode Continuation을 높이 평가합니다.
> 2026년 9월 29일~9월 30일 AI 뉴스입니다. 저희는 12개 서브레딧, 544개 트위터 계정을 확인했으며, 추가 디스코드는 확인하지 않았습니다. AINews 웹사이트에서 지난 모든 이슈를 검색할 수 있습니다. AINews는 이제 Latent Space의 한 섹션임을 알려드립니다. 이메일 수신 빈도를 선택/해제할 수 있습니다!

---

# AI 트위터 요약
Gemini 4 Argon: Google, 프론티어로 복귀
- 출시: Google DeepMind가 코딩, 기업 지식 작업 및 사이버 방어를 위한 Gemini 4 Argon을 소개했습니다 (@GoogleDeepMind, @sundarpichai).가용성: Fairwind Program의 정부 사용자 및 신뢰할 수 있는 사이버 방어자부터 접근이 시작됩니다. Google은 개발자, 기업 및 소비자에게 접근을 개방하기 전에 안전 장치를 다듬을 것이라고 밝혔습니다 (@Google, @demishassabis).출력 제한: Google은 업계 최고 수준인 1M 토큰 출력 제한을 언급했으며, 이는 64K에서 증가한 수치입니다 (@GoogleAI, @TheRundownAI).측정 참고: Vals는 최대 출력 262K를 기록했습니다. Artificial Analysis는 긴 응답을 일시 중지하고 호출을 통해 재개하는 새로운 API 기능인 Long Decode Continuation을 통해 1M 출력 토큰에 도달했습니다 (@ValsAI, @ArtificialAnlys).가격: 표준 가격은 1M 입력/출력 토큰당 $4/$20입니다. 50% 출시 기념 할인이 적용되어 $2/$10이며, 종료일은 발표되지 않았습니다. 캐시된 입력은 95% 할인을 받습니다 (@_philschmid, @ArtificialAnlys).
- Google의 주장하는 결과: Argon은 GPT-6 Astra 및 Claude Opus 5.5에 대한 19개 공개 벤치마크 중 13개에서 1위를 차지했습니다. DeepSWE에서는 77.9%를 기록했으며, Opus 5.5의 74.2% 및 Astra의 74.1%와 비교됩니다 (@TheRundownAI).내부 배포: Google은 Argon 에이전트가 300 TiB 이상의 데이터센터 메모리를 확보했으며, 80만 줄 이상의 C/C++ 커널 코드를 Rust로 마이그레이션하고 있다고 보고했습니다 (@kimmonismus).비디오 디코더: 에이전트들은 3만 2천 줄의 SIMD 코드를 안전한 Rust로 대체하여, 기존 Rust 포트를 동일한 출력으로 2.7배 빠르게 만들었습니다.연구 활용: 팀은 Argon을 기반으로 구축된 내부 에이전트 루프가 CK 추측을 완성하는 데 도움이 되었다고 밝혔습니다 (@mirrokni).
- Artificial Analysis 평가: Argon은 Intelligence Index에서 53점을 기록하여 GPT-6 Astra(53점)와 일치하고 GPT-6.1 Sol(52점)을 근소하게 앞섰습니다 (@ArtificialAnlys).작업당 비용: 할인 가격 적용 시 작업당 $1.99이며, Astra의 $3.26과 비교됩니다. 표준 가격으로는 $3.98로 상승할 것입니다.토큰 사용량: 절감 효과는 효율성이 아닌 가격에서 비롯됩니다. Argon은 작업당 평균 6만 2천 출력 토큰을 사용하는 반면 Astra는 2만 7천 토큰을 사용합니다.에이전틱 작업: AutomationBench-AA에서 77.5%로 1위를 차지했으며, Terminal Bench 4에서는 57%를 기록하여 Sonnet 5.5, Opus 5.5, Astra에 뒤처졌습니다.환각: AA-Omniscience에서의 환각 비율은 15%로, Astra의 51%와 비교됩니다. 절충점은 낮은 정확도입니다: 50% 대 Astra의 63%입니다 (@aipulseda1ly).
- Vals 평가: Argon은 Vals Index에서 68.9%로 1위를 차지했으며, 작업당 평균 $15.68입니다 (@ValsAI, @ValsAI).코딩: 30개의 Vibe Code Bench 앱을 완벽하게 구축했으며, Opus 5의 25개 및 Astra의 24개와 비교됩니다 (@ValsAI).터미널 및 보안: Terminal-Bench 4.0은 19.0%에서 57.6%로 상승했습니다. CyberBench 개념 증명 작업에서 70%를 기록했으며, IOI 2024–2026에서는 100%를 기록했습니다 (@ValsAI).효율성: Vals Index 작업에서 Sonnet 5.5의 출력 토큰의 약 4분의 1을 사용합니다 (@ValsAI).
- Arena 및 기타 평가: Argon은 Text Arena에서 1525점으로 1위, Code Arena WebDev에서 1679점으로 8위를 차지했습니다 (@arena).Agent Arena: 예비 3천 세션에서 전체 8위, 조종 가능성(steerability) 부문 1위를 기록했습니다 (@arena).PostTrainBench: 45.3%를 기록하여 Gemini 3.1 Pro의 21.99%에서 상승했습니다 (@karinanguyen).
- 회의론: 일부 관찰자들은 공개된 수치에 의문을 제기했습니다.법률 벤치마크: Argon이 Harvey의 법률 벤치마크에서 보고한 19.6%는 Muse Spark 1.2의 명시된 25.42%에 뒤처집니다 (@BlackHC).기타 비판: 논평가들은 선호도 데이터 벤치맥싱 가능성을 제기했으며, DeepSWE를 포함한 일부 수치에 이의를 제기했습니다 (@teortaxesTex, @teortaxesTex).
GPT-6.1 Sol 및 OpenAI의 DevDay 에이전트 스택
- 독립 평가: GPT-6.1 Sol은 MathArena에서 새로운 1위를 차지했습니다 (@j_dekoninck).Code Arena: WebDev에서 1759점으로 3위를 기록했으며, 동일한 $2/$10 가격으로 GPT-6 Sol보다 70점 앞섰습니다 (@arena).작업당 비용: Artificial Analysis는 최대 노력 시 작업당 $0.72로 측정했으며, Astra의 $3.26 및 GPT-6 Sol의 $1.04와 비교됩니다 (@ArtificialAnlys).절감의 원천: Sol은 더 적은 턴을 사용하고 캐시 읽기 가격이 더 낮습니다 (@ArtificialAnlys).Luna 버그 수정: OpenAI는 이미지 인코딩 버그를 수정하여 GPT-6 Luna에 Intelligence Index 1점을 추가했습니다.
- 초고속 인퍼런스: OpenAI는 최대 300 토큰/초를 언급했습니다. SemiAnalysis는 낮은 배치 크기에서 NVIDIA GPU로 실행되며 Cerebras에서는 실행되지 않는다고 보고했습니다 (@kimmonismus).실사용 보고서: 생성 속도는 약 8배 빠르지만, 툴 레이턴시가 지배적이므로 엔드투엔드 에이전트 작업은 2~4배만 빨라집니다 (@sayashk).컴퓨터 사용: UI 동작이 밀리초 단위로 반응하므로 여기서 이득이 가장 큽니다.비용: 테스터는 약 2시간 만에 주간 제한을 소진했습니다.
- 제품 레이어: DevDay는 dots(자체 클라우드 컴퓨터를 가진 영구 에이전트), Decisions API 및 컴퓨터 사용 기능을 소개했습니다 (@latentspacepod).사이트: ChatGPT Sites는 이제 MCP 서버를 호스팅하고 이를 설치 가능한 플러그인으로 전환할 수 있습니다 (@mxstbr).사용량 제한: 사용자들은 약 $2,500 상당의 일회성 크레딧을 보고했습니다. 다른 사용자들은 사용량 제한이 줄었다고 불평했습니다 (@kimmonismus, @kimmonismus).
기타 출시: 임베딩, 이미지/비디오 및 오픈 모델
- Perplexity 컨텍스트 임베딩: pplx-embed-v2-context-9b-preview가 Hugging Face에 공개되었습니다 (@perplexity_ai).방법: 이 모델은 전체 문서를 한 번 인코딩한 다음 청크 벡터를 풀링합니다. 학습은 단일 골드 청크 레이블을 사용하는 대신 컨텍스트 압축 모델에서 관련성을 디스틸레이션합니다 (@denisyarats).결과: ConTEB에서 새로운 최고 성능(SOTA)을 달성했습니다. turbopuffer의 비공개 컨텍스트 벤치마크에서는 8KB 대비 1KB int8 벡터를 사용하여 답변 recall@10에서 voyage-context-4를 14.4점 앞섰습니다 (@turbopuffer).
- Cohere Embed 5: 이 제품군은 공유 임베딩 공간에 Pro 및 Fast 변형을 가지고 있어, 하나로 인덱싱하고 다른 하나로 리트리벌할 수 있습니다 (@cohere).Fast 티어: Cohere는 다른 Fast 티어 모델보다 최소 6점 앞서며, Pro보다 3분의 1 적은 비용으로 제공된다고 밝혔습니다. 평가는 새로운 RCP-nDCG@10 메트릭을 사용합니다 (@cohere).
- Ideogram 4.5: 이 편집 모델은 아티팩트 없는 다중 턴 편집을 목표로 하며, 오픈 웨이트를 약속했습니다 (@ideogram_ai).편집 충실도: 10회 연속 편집 후에도 건드리지 않은 콘텐츠의 94~99%가 동일하게 유지됩니다 (@fal).순위: Image Edit Arena에서 1351점으로 18위를 차지했습니다 (@arena).
- 비디오 벤치마크: Artificial Analysis는 6만 8천 개 이상의 인간 투표로 1080p에서 평가된 AA-Video-T2V v2.0을 출시했습니다 (@ArtificialAnlys).선두 주자: Wan 3.0이 분당 $12로 1위입니다. Seedance 2.5는 분당 $34.12로 2위이며, MiniMax H3는 분당 $4.80로 통계적으로 동률입니다.Utopai X: MiniMax H3의 이 후속 학습(post-train) 모델은 2위로 데뷔했습니다 (@ArtificialAnlys).
- 오픈 및 소형 모델:Ling-3.1-flash: GPT-5.6 Sol 및 Opus 5에 근접한다고 보고된 500B 모델입니다 (@kimmonismus). Mobile App Arena에서 오픈 웨이트 모델 중 2위를 차지했습니다 (@DesignArena).Praxis-1: Runway는 오픈 웨이트 월드 액션 모델을 출시했으며, 로보틱스 정책 성능이 3인칭 비디오와 예측 가능하게 스케일링된다고 밝혔습니다 (@agermanidis).Solar Mini 4: Upstage는 총 350억 / 활성 30억 파라미터를 보고했습니다. Intelligence Index에서 $0.10/$0.40으로 24점을 기록했습니다 (@ArtificialAnlys).캐싱 페널티: 반복되는 컨텍스트의 48%만 캐시에 적중하는 반면 Luna는 99%이기 때문에, 작업당 Luna보다 여전히 약 5배 더 비쌉니다 (@ArtificialAnlys).
에이전트 연구, 인퍼런스 및 시스템
- 컨텍스트 언어 모델 (Meta): CLM은 컨텍스트를 추가 전용 로그가 아닌 편집 가능한 파일로 취급하며, 가중치에 학습된 컨텍스트 관리 정책을 사용하고 외부 하네스가 없습니다 (@RulinShao).결과: 24시간 멀티 리포지토리 에이전트 스웜 작업에서 동일한 컴퓨팅으로 65% 더 높은 점수를 기록했습니다 (@arankomatsuzaki, @natolambert).
- 적응형 추론 컴퓨팅:TaH2: 룩어헤드 뎁스 슈퍼비전은 모델에게 어떤 하드 토큰이 추가 루프를 받을 자격이 있는지 가르칩니다 (@ZhihuFrontier).이득: 일치하는 테스트 시간 컴퓨팅에서 정확도 3.4%p 증가와 53% 더 가파른 스케일링 슬로프를 보고합니다.서빙: MiniSGL 통합은 다른 루프 깊이의 요청을 함께 배치합니다.AutoBenchmark (Meta): 이 프로젝트는 벤치마크 생성을 자동화합니다. 아이디어 구상 단계에서의 인간 피드백이 에이전트 단독 작업보다 우수하며, 난이도가 보류된 솔버로 전이됩니다 (@jaseweston).Stratego: Nature 논문은 RL과 불완전 정보 하의 테스트 시간 컴퓨팅을 기반으로 구축된 최초의 초인적인 Stratego AI를 제시합니다 (@ssokota).
- 프리필/디코드 분리: 정상 상태 분석은 분리가 동일한 배치 크기와 처리량에서 평균 상호작용성을 약 1/(디코드 시간 비율)만큼 증가시킨다고 주장합니다 (@ekzhang1, @cHHillee).함의: 이는 프리필 위주 워크로드에 도움이 되며, 디코드 바운드 저 레이턴시 서빙에는 해당하지 않습니다.
- 컴파일러 및 하드웨어:Huawei의 DeepSeek: DeepSeek은 Ascend 950에 최적화된 TileLang을 포함한 오픈소스 Ascend 툴킷을 출시했습니다 (@kimmonismus).컴파일러로서의 AI: 모델이 Triton을 PTX로 직접 번역하며, 검증기가 정확성, 경쟁 조건 및 교착 상태를 확인합니다. B200에서 FlashAttention에 대한 속도 향상이 1.37배에 도달합니다 (@Azaliamirh).Vera Rubin: Cognition은 CoreWeave를 통해 Vera Rubin의 첫 고객이며, 동일한 디코드 속도에서 GB200의 토큰 처리량의 약 4.8배를 보고했습니다 (@cognition).DFlash 드래프트: Ornith-1.5의 새로운 드래프트 모델은 최대 2.54배의 무손실 속도 향상을 제공합니다 (@ornith_).
- 에이전트 샌드박스: Cloudflare는 에이전트용 컨테이너를 재구축했으며, p50 상호작용까지 걸리는 시간은 648ms (6배 빠름)이고 스냅샷은 베타 버전입니다 (@mgamache).AutoRouter: Cloudflare의 모델 라우터는 내부 테스트에서 약 30% 낮은 지출을 보였습니다 (@ashleypeacock).
안전성, 보안 및 평가 무결성
- 추론 추출: OpenAI는 숨겨진 추론 추출 캠페인의 핵심 부분이 Moonshot AI와 관련된 개인에게 있다고 지목했습니다 (@kimmonismus).규모: OpenAI는 이틀 동안 4천 명 이상의 사용자로부터 1만 6천 건의 시도를 기록했으며, 1만 5천 명 이상의 사용자에게서 관련 활동이 있었습니다.외부 연구자: 그들의 공격은 이번 주까지 Astra에서 계속 작동했습니다. 패치는 제품 버전 및 서드파티 호스트에 걸쳐 전파하기 어려웠습니다 (@JSchaeff3r, @jonasgeiping).비판: Nathan Lambert는 취약점은 API 제공자의 책임이라고 주장합니다 (@natolambert).
- 디스틸레이션 방어: 나중에 RL 없이 평가된 방어는 잘못된 보안 의식을 줍니다. RL은 단순 공격을 효과적으로 만듭니다 (@shidan_javaheri).
- 임베디드 평가: Apollo Research는 프론티어 랩에 직원과 유사한 접근 권한을 받는 외부 평가자를 위한 원칙을 발표했습니다 (@ApolloResearch).
- 사이버 평가: CyberGym-E2E-AA에서 일부 프론티어 모델은 85% 이상의 작업에서 안전성 차단됩니다 (@ArtificialAnlys).비용: GPT-6 Luna 또는 MiMo-V2.6-Pro는 약 $20로 100만 줄 코드베이스에서 약 100개의 버그 헌트를 실행할 수 있습니다.
- 출처 및 투명성:SynthID Bio: AI 생성 단백질에 대한 워터마킹이 Nature에 게재되었으며, 오픈소스 툴이 함께 제공됩니다 (@demishassabis).AI 탐지 회피: Opus 5.5 및 Astra는 Pangram이 플래그를 지정하지 않고 문서의 50% 이상을 다시 작성할 수 있습니다 (@ValsAI).에이전트 보고서: 새로운 프리프린트 논문은 LLM이 작성한 에이전트 작업 보고서가 실제로 얼마나 투명한지 질문합니다 (@jennyihuang).
산업 및 정책
- Factory 대 Cognition: Factory는 고문 Chris Degnan을 해임했으며, 그가 Cognition 이사회 회의에 참석하면서 Cognition에 기밀을 털어놓았다고 주장했습니다 (@matanSF).고용: Cognition은 같은 날 Degnan을 CRO로 발표했습니다 (@cognition).부인: Cognition의 CEO는 Factory 정보가 공유되지 않았으며 Degnan이 월요일에 고문직을 사임했다고 밝혔습니다 (@ScottWu46).
- 정치 자금 지출: Greg Brockman은 Leading the Future 슈퍼 PAC에 약속했던 두 번째 2,500만 달러 기부를 철회했습니다 (@teddyschleifer).후속 질문: Alex Bores는 이것이 기부자를 공개하지 않는 규제 반대 그룹도 포함하는지 질문했습니다 (@AlexBores).
- OpenAI 재정: NYT는 OpenAI가 연간 매출 700억 달러에 육박하며, 1조 4천억 달러 기업 가치로 300억 달러를 조달하기 위한 협상 중이며, IPO는 내년으로 연기되었다고 보도했습니다 (@srimuppidi).
- 자금 조달: 하드웨어 엔지니어링을 위한 AI 툴링을 구축하는 Flow는 7억 5천만 달러 기업 가치로 5천만 달러 시리즈 B 자금을 조달했습니다 (@parisingh).
(참여도 기준) 인기 트윗
- Gemini 4 Argon 소개; Fairwind를 통한 신뢰할 수 있는 테스터 롤아웃 — 44.6K
- Google: 1M 출력 제한을 가진 Argon — 36.5K
- Factory, Cognition 행위로 고문 해임 — 6.4K
- Artificial Analysis: Argon, Astra와 53점으로 일치 — 4.5K
- Cognition CEO, Factory의 주장에 이의 제기 — 3.8K
- Argon 에이전트, 300 TiB 메모리 확보 및 Rust 마이그레이션 추진 — 3.7K
- Ideogram 4.5, 정밀한 다중 턴 편집용 — 3.2K
- Arena: Argon, Text Arena에서 1위 — 3.0K

---

# AI Reddit 요약

## /r/LocalLlama + /r/localLLM 요약

### 1. GLM-5.3 사이버 리스크 및 로컬 인퍼런스 지원
- GLM-5.3 및 고급 사이버 역량 확산 \ Anthropic (활동: 785): Anthropic은 Zhipu/Z.ai의 오픈 웨이트 GLM-5.3이 자율 사이버 역량에 대한 주목할 만한 임계값을 초과했다고 보고했습니다: ExploitBench에서 50/410개의 엔드투엔드 V8 익스플로잇을 기록하여 Claude Mythos Preview의 56/410에 근접했으며, 이전 모델이 거의 0에 가까웠던 Anthropic의 내부 바이너리 익스플로잇 태스크의 4%에서 완전한 제어 흐름 하이재킹을 달성했습니다. Anthropic은 위험을 역량 + 접근성으로 구성합니다: GLM-5.3은 광범위하게 다운로드 가능하고, 비교적 저렴하며, 약하게 거부 튜닝되어 있으며, 단순한 탈옥이 64~100% 성공한다고 보고되었고, "어블리터레이션"은 측정된 역량 저하가 거의 없이 거부율을 한 자릿수로 낮춥니다. 상위 댓글들은 Anthropic의 구성에 대체로 적대적이었으며, 해당 게시물이 Anthropic의 프론티어에 근접한 더 저렴하고 오픈된 중국 모델을 억압하려는 시도로 읽힌다고 주장했습니다. 한 논평가는 합법적인 방어적 사용을 강조하며, GLM-5.3이 보안 테스트 및 자체 소프트웨어 개선을 위한 유일한 실용적인 도구라고 말했습니다.논평가들은 GLM-5.3을 프론티어 역량에 근접하다고 인식되는 저비용, 덜 제한적인 모델로 강조하며, 한 사용자는 이를 본질적으로 악의적이기보다는 "자체 소프트웨어의 보안 테스트 및 개선"에 유용하다고 구성했습니다. 제기된 기술적 우려는 Anthropic과 같은 제공업체의 제한이 잠재적으로 민감한 익스플로잇 또는 취약점 패턴을 분석하려는 모델을 필요로 하는 방어적 사이버 보안 워크플로우를 제한할 수 있다는 것입니다.한 논평가는 이전 GLM-5.2 모델이 Hugging Face 공격 완화에 도움이 되었다고 언급하며, Claude가 지원을 거부했다고 주장하는 것과 대조했습니다. 실질적인 요점은 거부 정책이 사고 대응 또는 취약점 완화 시나리오에서 유용성을 감소시킬 수 있는 반면, 더 관대한 모델은 방어적 보안 작업에 운영상 유용할 수 있다는 것입니다.
- timkhronos의 GLM-5.3-Flash (GLM5-Next) 지원 추가 · Pull Request #27773 · ggml-org/llama.cpp (활동: 348): 병합된 ggml-org/llama.cpp#27773은 llama.cpp에 GLM-5.3-Flash / GLM5-Next 지원을 추가하여 320B 하이브리드 텍스트+비전 모델에 대한 로컬 인퍼런스를 가능하게 합니다. 이 구현은 GLM 특정 DSA 인덱싱/풀링, 하이브리드 인덱스드 메모리, 새로운 glm5v 비전 전처리/타워 경로를 추가하는 동시에 Kimi-K3 KDA 레이어, DeepSeek 스타일 MoE/mHC 헬퍼, MLA 전용 어텐션, DSV4 스타일 SwigLU 클램핑을 재사용합니다. 검증 보고서는 프리필/유배칭/디코드 전반에 걸쳐 Transformers와 일치하는 랜덤 모델 로짓과 약 1e-5의 비전 임베딩 일치를 보고하며, 일부 정밀도 민감 텐서는 비양자화 상태로 남겨졌습니다. 논평가들은 llama.cpp 모델 지원이 새로운 실험적 아키텍처의 속도를 따라가지 못하는 것에 우려를 표했으며, 한 논평가는 실질적인 병목 현상이 관리자 가용성으로 보인다고 언급했습니다. 기술적 호환성 문제도 제기되었습니다: 기존 Unsloth 양자화는 glm5next를 사용하는 반면 메인라인은 glm5-next를 예상한다고 보고되었으므로, 현재 메인라인은 해당 양자화를 로드하지 못할 수 있습니다.논평가들은 Unsloth 양자화 PR과 메인라인 llama.cpp PR 간의 호환성 문제를 지적했습니다: 하나는 아키텍처/모델 타입을 glm5next로 식별하고 다른 하나는 glm5-next를 사용하는데, 이는 메인라인 llama.cpp가 변환 또는 메타데이터 수정 없이 기존 Unsloth GLM-5.3-Flash 양자화를 로드하지 못할 수 있음을 의미합니다.llama.cpp 지원이 새로운 모델 출시 속도를 따라가지 못하는 것에 대한 우려가 있었습니다. 특히 새로운 모델들이 인퍼런스 및 최적화 작업이 적용되기 전에 맞춤형 로더/런타임 변경을 요구하는 실험적 아키텍처를 점점 더 많이 사용함에 따라 이러한 우려가 커졌습니다. 한 논평가는 GLM-5.3-Flash 지원이 모델 출시 후 대략 "한 달 더" 걸린다고 구성했으며, 진행 상황이 소수의 관리자에게 크게 의존한다고 언급했습니다.

## 7일 무료 체험으로 계속 읽기
Latent.Space를 구독하여 이 게시물을 계속 읽고 전체 게시물 아카이브에 7일간 무료로 액세스하세요.
[체험 시작](https://www.latent.space/subscribe?simple=true&next=https%3A%2F%2Fwww.latent.space%2Fp%2Fainews-gemini-4-argon-gdms-answer&utm_source=paywall-free-trial&utm_medium=web&utm_content=218294409&coupon=5fe099d9)[이미 유료 구독자이신가요? 로그인](https://substack.com/sign-in?redirect=%2Fp%2Fainews-gemini-4-argon-gdms-answer&for_pub=swyx&change_user=false)

---

*이 문서는 Latent Space AINews 뉴스레터를 자동 번역한 것입니다.*
